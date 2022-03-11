# Helm Repo

To add a new chart:
1. Add the remote chart repository to your local helm `helm repo add <repo-name> <repo-location>`
2. Package a chart to a tgz file with `helm package <chart-name> --version <chart-version>`
3. Place the tgz file on the root of this repo.
4. Run `helm repo index --url https://dixahq.github.io/sre-helm-repo/ .`, which will update `index.yaml` with a new Chart entry.
5. Push changes to `main`, which will publish the Chart.
6. Remember to run `helm repo update` to fetch updates to `sre-helm-repo`.
