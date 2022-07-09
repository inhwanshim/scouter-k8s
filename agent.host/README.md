# scouter-k8s

## agent.host

* namespace: kube-system
* resources
  * configmap
  * daemonset

* how to use
  * edit scouter.conf
  * verify

    ```
    $ kubectl kustomize
    ```

  * apply

    ```
    $ kubectl apply -k .
    ```
