# exp-gitops-v1

argocd app create example-app \
 --repo https://github.com/meabhishekkumar/exp-gitops-v1.git \
 --path charts/guestbook \
 --dest-server https://kubernetes.default.svc \
 --dest-namespace default

argocd app sync example-app
