# OU-110-CustomDashboardConfigMap
Example for creating a custom dashboard within OpenShift > Observe > Dashboards

 1. Sign into a cluster as an administrator </br>
 2. For a dashboard to appear in the Console UI, the dashboard definition JSON needs to be loaded into a ConfigMap in the `openshift-config-managed` namespace. </br>
  `oc project openshift-config-managed` </br>
  `oc apply -f jz-dashboard-configMap-120522` </br>
  `$ configmap/jz-custom-dashboard-config-121322 created` </br>
 3. Check if configMap has been applied `jz-custom-dashboard-config-121322` should now be listed among the configmaps. </br>
  `oc get configmaps` </br>
