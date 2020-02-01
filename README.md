1. Make sure a kubernetes cluster is up and running and you have kubectl installed

2. run busybox container in pod
    ```
    $ kubectl apply -f busybox.yaml
    ```

3. execute nslookup in busybox pod
	```
	$ kubectl -n default exec -ti busybox-pod -- nslookup <svc-name>
	```