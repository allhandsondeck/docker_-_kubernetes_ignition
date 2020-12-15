# docker_kubernetes_ignition

This is my first attempt to try out docker and kubernetes together.

Install `express` for server.

_$ npm install_

Build the image:

_$ docker build -t node-web-app ._

Execute deployment.yaml:

_$ kubectl apply -f application/deployment.yaml_

Deploy the service:

_$ kubectl apply -f application/service.yaml_

To check if service is running:

_$ kubectl describe svc my-service-for-my-webapp_

Now, you can open http://localhost:80

To clear deployments:

_$ kubectl delete -f ./application/service.yaml_

_$ kubectl delete -f application/deployment.yaml_
