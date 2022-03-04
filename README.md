# ansible-playbook-challenge-3
# class challenge creating ansible playbook to parse data from web service and into remote node
# this anisble playbook is created by masnawi rahmat in submission of class challenge no 3 
# in Generation SG/Temasek Poly SGUPMSCT Cloud Support and DevOPs Bootcamp cohort no 4 Yr 2022
# this ansible playbook assumes that you:
# (1) have the NOPASSWD auth in the remote node to execute commands otherwise please insert line 
# "your_username" ALL=(ALL:ALL)       NOPASSWD: ALL" in /etc/sudoers.d
# (2) have jmespath package installed to execute 'jmesquery' otherwise do a 'pip install jmespath' 
# the objectives of this ansible playbook:
# (1) fetch data from data.gov.sg api
# (2) parse and save json data file
# (3) calculate the sum of uni/poly IT graduates from yyyy to yyyy 
# tasks covered in this playbook: 
# (1) creating directory and subdirectories by looping
# (2) fetching and saving data from data.gov.sg api into a file
# (3) parsing json data with jmespath and json_query
# (4) saving parsed data into a new file  
# (5) calculating the sum of uni/poly IT graduates and writing the value into a pre-existing file
# (6) optional - removing all directory, subdirectories and files created by this ansible playbook
# and to activate, please 'uncomment' line 104 to 114
