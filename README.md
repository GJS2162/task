### **Pre-requisites**

- Make sure you have a running Kubernetes cluster (using kind, Minikube, or any other solution).  
- Ensure `helm` and `kubectl` are installed and configured.

### **Deployment**

To deploy the application using the Helm chart, run the following commands:

1. **Install the Helm chart**:
   ```bash
   helm install testapp cosmocloud-deploy --atomic --timeout 30s
   ```

2. **Verify the deployment**:
   ```bash
   kubectl get pods
   kubectl get services
   ```

3. **Uninstall the deployment**:
   ```bash
   helm uninstall testapp
   ```
