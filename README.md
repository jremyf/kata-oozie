# Kata-oozie

You first need to create a job.properties file to configure your oozie workflow.

You also  need to push all the needed file (workflow.xml / hive-site.xml / hive.hql) to your personal HDFS folder using :

`hdfs dfs -copyFromLocal "file"`

Then, run the following command to execute your workflow :

`oozie job -oozie http://sandbox-hdp.hortonworks.com:11000/oozie -config job.properties -run`

Next you can check on the Oozie webpage the execution of your workflow :

http://sandbox-hdp.hortonworks.com:11000/oozie









