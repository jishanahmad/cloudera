# Ranger
* Is used for Autherisation
* [Installing Ranger in CM](../documents/mod19_ex01__installing_ranger.pdf)
* [Configuring Ranger in CM](../documents/mod19_ex02__configuring_ranger.pdf)
* [Installing Ranger RMS](../documents/mod19_ex03__installing_ranger_rms.pdf)
   * Legacy CDH users set Hive policies which automatically linked Hive permissions to HDFS ACL's. 
   * This was especially convenient for external table data used by Spark or Hive. 
   * Previously, Ranger managed Hive and HDFS policies separately, you had to set both. 
   * Ranger RMS replicates the CDH capability, setting a Hive policy will make changes in HDFS. 
