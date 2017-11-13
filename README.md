Docker - Tomcat with Oracle JDK
=================
### Prepare ROOT.war in webapps
```
lucas@machine:~/Desktop$ ls -l webapps/
total 47484
-rw-r--r-- 1 root root 48619943  8   1 10:31 ROOT.war
```


### Put ROOT.war into container

```sh
docker run -p 8080:8080 -v $PWD/webapps:/opt/tomcat/webapps -it lucasko/tomcat
```










