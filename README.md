# ELK  

## Check ELK stack state by executing docker-compose ps  
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/docker%20ps.PNG)  

### Put global index settings with ./put.sh global.json  

### Put template for deployments index by executing ./put.sh deployments.json  
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/put.sh.PNG)  
 
##### !Use   
``` sed -i -e 's/\r$//' scriptname.sh ```  
##### if you have  '/bin/bash^M: bad interpreter: No such file or directory'!  
  
 
### Deploy first version of application   
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/first%20release.PNG)  

### Here the first Kibana page  

 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/kibana%20show%20page.PNG)

### Creating index pattern
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/logstash%20create.PNG)

###  Choose visualisation  
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/visualization.PNG)
 
### Add settings for graph construction
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/1st%20deploy%20visual.PNG)

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
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/dock%20pull%20metri.PNG)

### Configure Metricbeaton Docker
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/example%20config%20file.PNG)
 
### Volume-mounted configuration
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/volume-mounted.PNG)
 
### Customize configuration
 ![alt-текст](https://github.com/KaterynaKalinichenko/ELK/blob/master/images/metr/customize.PNG)


 
 