\# ansible-playbook-challenge-3a <br />
\# class challenge creating ansible playbook to parse data from web service and into remote node <br />
\# this ansible playbook is created with learning purpose more than optimisation in mind <br />
\# this anisble playbook is created in submission of class challenge no 3 <br />
\# in Generation SG/Temasek Poly SGUPMSCT Cloud Support and DevOps Bootcamp cohort no 4 Yr 2022 <br />
\# this ansible playbook assumes that you: <br />
\# (1) have the NOPASSWD auth at the remote node to execute commands otherwise please insert line <br />
\# "your_username" ALL=(ALL:ALL)       NOPASSWD: ALL" in /etc/sudoers.d <br />
\# (2) have jmespath package installed at the control node to execute 'jmesquery' otherwise do a 'pip/apt install jmespath' <br />
\# the objectives of this ansible playbook: <br />
\# (1) fetch data from data.gov.sg api <br />
\# (2) parse and save json data file <br />
\# (3) calculate the sum of uni/poly IT graduates from yyyy to yyyy <br />
\# tasks covered in this playbook: <br />
\# (1) creating directory and subdirectories by looping <br />
\# (2) fetching and saving data from data.gov.sg api into a file <br />
\# (3) parsing json data with jmesquery and json_query <br />
\# (4) saving parsed data into a new file <br />
\# (5) calculating the sum of uni/poly IT graduates and writing the value into a pre-existing file <br />
\# (6) optional - removing all directory, subdirectories and files created by this ansible playbook and to activate, please 'uncomment' line 105 to 115
