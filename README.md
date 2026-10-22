# aws-gitops

Argo CD app-of-apps for the devops-lab EKS cluster.

- `root.yaml` – the one file applied by hand (`kubectl apply -f root.yaml`); watches `apps/`
- `apps/` – one Argo CD `Application` per workload
- `demo-app/` – manifests for [aws-demo-app](https://github.com/Most-Fullstack/aws-demo-app); bump the image tag in `deployment.yaml` after each build
