# Tutorial 11

1. Compare the application logs before and after you exposed it as a Service.
Try to open the app several times while the proxy into the Service is running.
What do you see in the logs? Does the number of logs increase each time you open the app?

![alt text](log-before.png)

![alt text](log-after.png)

- Before exposing the service, the log only shows which port the server is on. After the exposal of the service, it began logging the requests. Those requests can be seen in the logs as shown in the picture above.

2. Notice that there are two versions of `kubectl get` invocation during this tutorial section. he first does not have any option, while the latter has `-n` option with value set to
 `kube-system`.
 What is the purpose of the `-n` option and why did the output not list the pods/services that you
 explicitly created

- The -n stands for namespace. -n kube-system means instruct the terminal to search for the service with the namespace -n -kube-system.

