* kubectl do not print the headers like when you want to pipe to wc -l **--no-headers**
* to see all the yaml options use the ```explain --recursive``` switch e.g. ```kubectl explain pod --recursive ``` add grep Ax to view x lines below the grep result



    * all
    * certificatesigningrequests (aka 'csr')
    * clusterrolebindings
    * clusterroles
    * clusters (valid only for federation apiservers)
    * componentstatuses (aka 'cs')
    * configmaps (aka 'cm')
    * controllerrevisions
    * cronjobs
    * customresourcedefinition (aka 'crd')
    * daemonsets (aka 'ds')
    * deployments (aka 'deploy')
    * endpoints (aka 'ep')
    * events (aka 'ev')
    * horizontalpodautoscalers (aka 'hpa')
    * ingresses (aka 'ing')
    * jobs
    * limitranges (aka 'limits')
    * namespaces (aka 'ns')
    * networkpolicies (aka 'netpol')
    * nodes (aka 'no')
    * persistentvolumeclaims (aka 'pvc')
    * persistentvolumes (aka 'pv')
    * poddisruptionbudgets (aka 'pdb')
    * podpreset
    * pods (aka 'po')
    * podsecuritypolicies (aka 'psp')
    * podtemplates
    * replicasets (aka 'rs')
    * replicationcontrollers (aka 'rc')
    * resourcequotas (aka 'quota')
    * rolebindings
    * roles
    * secrets
    * serviceaccounts (aka 'sa')
    * services (aka 'svc')
    * statefulsets
    * storageclasses
