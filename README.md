## K8S manifests generated using Copilot

```
Note: kubectl-ai seems for me outdated and not maintained anymore. So I decided to use Copilot to generate K8S manifests.
```


| Name | Prompt | Description | Example |
|------|--------|-------------|---------|
| Pod | Generate k8s pod manifest for the demo app following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Pod manifest for the demo app. | [app.yaml](./yaml/app.yaml) |
| Pod with Liveness Probe | Generate k8s pod manifest with liveness probe for the demo app following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Pod manifest with liveness probe for the demo app. | [app-livenessProbe.yaml](./yaml/app-livenessProbe.yaml) |
| Pod with Readiness Probe | Generate k8s pod manifest with readiness probe for the demo app following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Pod manifest with readiness probe for the demo app. | [app-readinessProbe.yaml](./yaml/app-readinessProbe.yaml) |
| Pod with mounted volume | Generate k8s pod manifest with mounted volume for the demo app following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Pod manifest with mounted volume for the demo app. | [app-volumeMounts.yaml](./yaml/app-volumeMounts.yaml) |
| Cron job | Generate k8s cron job manifest example following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Cron Job manifest example. | [app-cronjob.yaml](./yaml/app-cronjob.yaml) |
| Job | Generate k8s job manifest example following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Job manifest example. | [app-job.yaml](./yaml/app-job.yaml) |
| Multi-container Pod | Generate k8s Multi-container Pod manifest with init container for db migrations for the demo app following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Multi-container Pod manifest for the demo app with an init container for DB migrations. | [app-multicontainer.yaml](./yaml/app-multicontainer.yaml) |
| Pod with resource limits | Generate k8s Pod manifest with resource limits for the demo app following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Pod manifest for the demo app with resource limits. | [app-resources.yaml](./yaml/app-resources.yaml) |
| Pod with secrets | Generate k8s Pod manifest with secrets for the demo app following naming best practices. Make sure all required fields are populated, provide one sentence description and name | Kubernetes Pod manifest for the demo app with secrets. | [app-secret-env.yaml](./yaml/app-secret-env.yaml) |
