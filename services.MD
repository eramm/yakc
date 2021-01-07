NODE PORT

**targetPort**

**port**

**nodePort**

kind: Service

type: NodePort

ports:

    - targetPort: 80 <-- port that the service uses

     port: 80 <-- mandatory <-- will be the same as targetPort if not specified

     nodePort: 30008 <-- user facing port <-- will be assigned automaticly if none specifed

    kk expose deploy simple-webapp-deployment --name=simple-webapp --port=8080 --target-port=8000 -l 'app=simple-web' --type='NodePort' --dry-run=client-o yaml > ./srv.yml

CLUSTER PORT

**targetPort**

**port**

**ONLY !**

groups pods with the same label into one "cluster" for service to service communication. INTERNAL ONLY)

you probaly only need to set the port 

   type: ClusterIP

   ports:

    - targetPort: 80 <-- port that the service uses

       port: 80 <-- port that the cluster will listen on


LOAD BALANCER

    type: LoadBalancer

    - targetPort: 80 <-- pod side port
      
      port <-- LB pod facing port
      
      nodePort: 30008 <-- public facing port

