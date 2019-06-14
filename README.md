# ELK  

## Check ELK stack state by executing docker-compose ps  

 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/docker%20ps.PNG)  
###### When we see that everything is running, we proceed to the next step.

### Put global index settings with ./put.sh global.json  
### Put template for deployments index by executing ./put.sh deployments.json  
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/put.sh.PNG)  
 
##### !Use
``` sed -i -e 's/\r$//' scriptname.sh ```  
##### if you have  '/bin/bash^M: bad interpreter: No such file or directory'!  
  
### Deploy first version of application   
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/first%20release.PNG)  
###### When we see that all the petshop components are running, we can check the result of our work.

### Here the first Kibana page  
###### Go to the Kibana main page and check that it works and we can perform actions with it.
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/kibana%20show%20page.PNG)

### Creating index pattern
###### We will work with patterns
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/logstash%20create.PNG)

###  Choose visualisation  
###### We need to choose the most convenient visualization. For me personally, this is exactly its "line".
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/visualization.PNG)
 
###### Add settings for graph construction
 ![alt-текст]()
###### And and build a beautiful graph
![alt-текст]()



##  Filebeat installation for Nginx

### First we need to install filebeat 
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/install%20fileb2.PNG)
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/install%20fileb3.PNG)
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/install%20file4.PNG)

### Check our module list 
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/nginx%20list.PNG)
### Enable the nginx module
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/enable%20ng.PNG)
 
### Check the configuration file is syntactically correct
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/check%20correct.PNG)
 
### Start adn enable filebeat
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/enable%20%26%26%20start%20filebeast.PNG)

# Install Metricbeat

 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/install%20metri.PNG)

## Running Metricbeat on Docker

### Pulling the image  
##### Obtaining Beats for Docker is as simple as issuing a simplest command against the Elastic Docker registry.

 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/dock%20pull%20metri.PNG)

### Configure Metricbeaton Docker
##### The Docker image provides several methods for configuring Metricbeat. The conventional approach is to provide a configuration file via a volume mount, but it’s also possible to create a custom image with your configuration included
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/example%20config%20file.PNG)
 
### Volume-mounted configuration
##### We can configure Metricbeat on Docker is to provide metricbeat.docker.yml via a volume mount..
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/volume-mounted.PNG)
 
### Customize configuration
###### The metricbeat.docker.yml file is configured to deploy Beats modules based on the Docker labels applied to your containers.
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/customize.PNG)


 
 