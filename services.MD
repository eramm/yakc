NODE PORT

**targetPort**
**port**
**nodePort**

kind: Service
type: NodePort
ports:
 - targetPort: 80
   port: 80 <-- mandatory <-- will be the same as targetPort if not specified
   nodePort: 30008 <-- user facing port <-- will be assigned automaticly if none specifed
