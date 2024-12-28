Deploy the different folders by creating an argocd app with the CLI
```bash
argocd app create example02 --repo https://github.com/vramahandry/gitops-cert-level-2-examples.git --path ./sync-hooks-waves/02-presync-job --dest-namespace example02 --dest-server https://kubernetes.default.svc --sync-policy none
```