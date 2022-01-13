# Helm Repo

To add a new chart:
1. Place the tgz file on the root of this repo.
2. Run `helm repo index --url https://dixahq.github.io/sre-helm-repo/ .`, which will update `index.yaml` with a new Chart entry.
3. Push changes to `main`, which will publish the Chart.
4. Remember to run `helm repo update` to fetch updates to `sre-helm-repo`.
