# k8s-kind-nodeport
Example code to deploy a simple nginx container into a kind kubernetes cluster using nodeport

## How to run this example
First you need to create the kubernetes cluster, we are gonna use kind tool to do it.
Make sure you have kind installed in your computer. You can check how to do it in the link below.
[Kind website](https://kind.sigs.k8s.io/).

Once you have kind installed, you need to run this command:  
`kind create cluster --name lab --config kind/config.yaml`

This command will take some time to finish, so you can get a coffee :)
Once you have your coffee and it is done, you need to run this command below.  
`kubectl apply -f k8s/nginx.yaml`

Once this command finishes, you can go to your browser and access localhost on port 80.  
[localhost](http://localhost:80)
