# ansible-playbook-challenge-3a
# class challenge creating ansible playbook to parse data from web service and into remote node
# this ansible playbook is created with learning purpose more than optimisation in mind
# this anisble playbook is created by masnawi rahmat in submission of class challenge no 3 
# in Generation SG/Temasek Poly SGUPMSCT Cloud Support and DevOps Bootcamp cohort no 4 Yr 2022
# this ansible playbook assumes that you:
# (1) have the NOPASSWD auth at the remote node to execute commands otherwise please insert line 
# "your_username" ALL=(ALL:ALL)       NOPASSWD: ALL" in /etc/sudoers.d
# (2) have jmespath package installed at the control node to execute 'jmesquery' otherwise do a 'pip/apt install jmespath' 
# the objectives of this ansible playbook:
# (1) fetch data from data.gov.sg api
# (2) parse and save json data file
# (3) calculate the sum of uni/poly IT graduates from yyyy to yyyy 
# tasks covered in this playbook: 
# (1) creating directory and subdirectories by looping
# (2) fetching and saving data from data.gov.sg api into a file
# (3) parsing json data with jmesquery and json_query
# (4) saving parsed data into a new file  
# (5) calculating the sum of uni/poly IT graduates and writing the value into a pre-existing file
# (6) optional - removing all directory, subdirectories and files created by this ansible playbook
# and to activate, please 'uncomment' line 105 to 115
