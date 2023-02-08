# OU-110-CustomDashboardConfigMap
Example for creating a custom dashboard within OpenShift > Observe > Dashboards

 1. Sign into a cluster as an administrator </br>
 2. For a dashboard to appear in the Console UI, the dashboard definition JSON needs to be loaded into a ConfigMap in the `openshift-config-managed` namespace. </br>
  `$oc project openshift-config-managed` </br>
  `$oc apply -f JZ-OU110-test-customDataSource-VariableDropDown-And-Panels` </br>
 3. Check if configMap has been applied `JZ-OU110-test-customDataSource-VariableDropDown-And-Panels` should now be listed among the configmaps. </br>
  `$oc get configmaps` </br>

### Prerequisite 
1. 'oc' Openshift CLI must be installed 
2. You must have administrator access to an OpenShift Cluster 
3. If you're running OpenShift CRC -- you must enable monitoring (its off but default to conserve resources). 
