Unlocking the World of Kubernetes: A Quick Start!

Embarking on the Kubernetes journey? 🌐 Let's make it a breeze! 🚀

For macOS Users:

To Install kubectl --> Command line tool for interacting with Kubernetes cluster.
brew install kubectl
To Install minikube --> Tool to run single node Kubernetes cluster locally
brew install minikube

To start minikube at the local machine
minikube start
To verify that minikube is running
kubectl get nodes

Create the helloworld.yaml file in your local machine and add the content from the attached file, the HelloWorld code, which we will deploy on the Kubernetes cluster.

To deploy the code
kubectl create -f helloworld.yaml
To see all resources created by the above cmd--> Pod, Service, Deployment, Replicaset
kubectl get all

So, now all resources for our application are created, but to access that application, we have to create a service.

To create a ‘NodePort’ service for helloworld deployment
kubectl exposes deployment helloworld —type=NodePort
NordPort: Make service accessible on IP at a static port allocated by Kubernetes

Now, to access the website.
minikube service helloworld

This will redirect you to your webpage, which is deployed on the Kubernetes cluster, minikube.

Ready to shine in the Kubernetes galaxy! 🚀✨ Share your 'Hello, World!' moment below and let the Kubernetes adventure begin! 👩‍💻👨‍💻 #KubernetesMagic #HelloWorld #TechJourney 🌟
