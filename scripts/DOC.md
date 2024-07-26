## Super duper script
To add a Bash script as a plugin to kubectl, you need to follow a specific naming convention and place the script in a directory that is included in your PATH. kubectl plugins are executable files whose names start with kubectl-. Here are the steps to achieve this:

**Rename the Script.** Rename your script to follow the kubectl-<plugin-name> format. For example, if you want to name your plugin top-resources, rename your script to kubectl-top-resources:

```bash
cp kubeplugin kubectl-rtop
```

**Make the Script Executable.** Ensure the script has execute permissions:

```bash
chmod +x kubectl-rtop
```

**Place the Script in Your PATH.** Move the script to a directory that is included in your PATH. For example, you can move it to /usr/local/bin:

```bash
sudo mv kubectl-rtop /usr/local/bin/
```

**Verify the Plugin** You can now run your script as a kubectl plugin:

```bash
kubectl plugin list
kubectl rtop <namespace> <resource-type>
```

Example output for `kube-system` namespace:

```bash
kubectl rtop kube-system
```

```
pod, kube-system, coredns-6799fbcd5-k5j27, 2m, 15Mi
pod, kube-system, local-path-provisioner-6f5d79df6-rnbvw, 1m, 27Mi
pod, kube-system, metrics-server-54fd9b65b-rtgn7, 4m, 51Mi
pod, kube-system, svclb-traefik-6abe5921-2strz, 0m, 0Mi
pod, kube-system, traefik-7d5f6474df-k4d55, 1m, 29Mi
```