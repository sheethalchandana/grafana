installation and setting up of GRAFANA in local environment
step 1: in AWS create an EC2 instance
step 2: enable port 3000 in the security groups
step 3: SSH the server
step 4: download GPG keys and add them to trusted keys list
        (#wget -q -O - https://packages.grafana.com/gpg.key | sudo apt-key add)
step 5: add GRAFANA repository
        (#sudo add-apt-repository "deb https://packages.grafana.com/oss/deb stable main")
step 6: update the system 
        (#sudo apt update)
step 7: install GRAFANA
        (#sudo apt install grafana)
step 8: add GRAFANA to auto start and start the grafana daemon itself
        (#sudo systemctl enable grafana-server)
        (#sudo systemctl start grafana-server)
step 9: check the status
        (#sudo systemctl status grafana-server)
step 10: go to browser and search with public ip of EC2  
        <public ip of EC2:3000> 
        
        
