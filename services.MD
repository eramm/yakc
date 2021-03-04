NODE PORT

**targetPort**

**port**

**nodePort**

kind: Service

type: NodePort

ports:

    - port: 80 <-- mandatory <-- will be the same as targetPort if you do not specify a target port 
    - targetPort: 80 <-- port that the pod service uses
    - nodePort: 30008 <-- user facing port <-- will be assigned automaticly if none specifed

     

    k expose deploy simple-webapp-deployment --name=simple-webapp --port=8080 --target-port=8000 -l 'app=simple-web' --type='NodePort' --dry-run=client-o yaml > ./srv.yml
    ```k create service nodeport --tcp=80:80

CLUSTER PORT

**targetPort**

**port**

**ONLY !**

groups pods with the same label into one "cluster" for service to service communication. INTERNAL ONLY)

you probaly only need to set the port 

   type: ClusterIP

   ports:

    - targetPort: 80 <-- port that the pod service uses

       port: 80 <-- port that the cluster will listen on


LOAD BALANCER

    type: LoadBalancer

    - targetPort: 80 <-- pod side port
      
      port <-- LB pod facing port
      
      nodePort: 30008 <-- public facing port

