# scouter-k8s

## agent.host

* namespace: scouter
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
