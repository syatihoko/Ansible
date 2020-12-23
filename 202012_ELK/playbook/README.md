# **README**  

**Usage:**  
    Playbook Installs and configures elasticsearch, kibana, logstash.  
    Creates basic configuration files for these services.  

**General variables:**  



| Group of variables           | Variable                | Variables value      
| ---------------------------- | ----------------------- |------------------------------------------ |
| group_vars/all/vars          | java_jdk_version        | version of JDK (default 11.0.9)           |
| group_vars/all/elasticsearch | elastic_version         | version of Elasticsearch (default 7.10.1) |
| group_vars/all/kibana        | kibana_version          | version of Kibana (default 7.10.1)        |
| group_vars/all/logstash      | logstash_version        | version of Logstash(default 7.10.1)       |

​           

**Groups:**  



| Groups        | Description           |
| ------------- | --------------------- |
| all           | install Java JDK      |
| elasticsearch | install elasticsearch |
| kibana        | install kibana        |
| logstash      | install logstash      |

**Host setup:**  
    By default, the stack exposes the following ports:  
    5044: Logstash Beats input  
    5000: Logstash TCP input  
    9600: Logstash monitoring API  
    9200: Elasticsearch HTTP  
    9300: Elasticsearch TCP transport  
    5601: Kibana  



**Tags:**



| Tag name      | Description                                               |
| ------------- | --------------------------------------------------------- |
| java          | Tasks for install Java JDK                                |
| elasticsearch | Tasks for install elasticsearch                           |
| kibana        | Tasks for install kibana                                  |
| logstash      | Tasks for install logstash                                |
| service       | Tasks for creating only service unit files from Templates |
| config        | Tasks for updating only config files from Templates       |

