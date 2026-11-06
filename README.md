# Repozytorium GitOps (źródło prawdy dla Argo CD)

To jest zawartość, którą w zadaniu P2 wypychasz do **własnego** repozytorium Git. Argo CD czyta z niego manifesty i pilnuje, żeby klaster wyglądał tak samo.

```text
apps/
└── web/              aplikacja z zadań P2-P4 (nginx, ConfigMap z podstroną, Service)
    ├── configmap.yaml
    ├── deployment.yaml
    └── service.yaml
```

W katalogu nie ma pliku `Namespace`: Argo CD tworzy go sam (`CreateNamespace=true` w `Application`).
