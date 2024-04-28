# jinja_renderer_app
jinja_renderer_app

docker build -t muzammilpeer/jinja-render-app:latest .
docker push muzammilpeer/jinja-render-app:latest
kubectl apply -f frontend-deployment.yaml


kubectl get all

# smart refresh
kubectl set image deployment/jinja-render-app nginx=muzammilpeer/jinja-render-app:latest
