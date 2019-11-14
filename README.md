# Spark --- for linux version greater than 14
Initial Commit

Step 1) First of all create a spark user(sudo) in the machines which are used in this setup.
        For that follow the link below:-
        https://www.digitalocean.com/community/tutorials/how-to-create-a-sudo-user-on-ubuntu-quickstart  

Step 2) a:- Installation for multinode:-
            Follow the link given
            https://data-flair.training/blogs/install-apache-spark-multi-node-cluster/
        b:- Follow the link below to install java
            https://tecadmin.net/install-oracle-java-8-ubuntu-via-ppa/
  
The above setup which is made by following the steps will create a multinode setup but the workers wont be shown in http://<master ip>:8080/ 
So insert the following line in /conf/spark-env.sh
    SPARK_MASTER_HOST=(master)
