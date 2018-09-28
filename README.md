
```
1)	Create a Name Space to hold service account 
               To create a name space with name “test-serviceaccount”
# kubectl create namespace test-serviceaccount 
2)	 Create a service account
To Create a service account with name “test-serviceaccount”
# kubectl create sa reader-1 -n test-serviceaccount
3)	Grant Cluster read access for the service account
# kubectl create clusterrolebinding reader-1 --clusterrole=view --serviceaccount=test-serviceaccount:reader-1 
4)	 kubectl get sa reader-1 -o yaml | grep –A3 ‘secrets:’ -> to list the secrets part of the Service Account
5)	 To get the token of the secret 
# kubectl get secrets reader-1-token-k54fn -o yaml | grep tocken:

# This token can be used in your API calls.



```
