Commands:

kubectl create namespace blog

https://portworx.com/run-ha-mariadb-google-kubernetes-engine/
V5PaJVPTX1

kubectl exec -it  ghost-mariadb-0 -- mysql -u root -p password

The below command is used to install our GHOST instance:

helm upgrade --install ghost C:\Users\Gilbert\Desktop\projects\github\gilbertblog\ghost --set service.type=LoadBalancer --set ghostPassword=xxxx --set mariadb.auth.rootPassword=xxxx --set mariadb.rootUser.password=xxxx,ghostHost=192.168.34.5,ghostPassword=xxxx,mariadb.db.password=xxxxx

SSL cert:
openssl req -newkey rsa:2048 -keyout ghdevopstechblog.hopto.org.key -out ghdevopstechblog.hopto.org.csr