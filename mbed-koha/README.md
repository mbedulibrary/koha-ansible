<h1>ANSIBLE PLAYBOOK FOR CENTOS 7 AND KOHA 17</h1> 
<h3>(based on https://github.com/nemobis/beic-koha)</h3>

<ol>
  <li>Install Core CentOS 7 – Connect to Network, set hostname, set time zone, make partitions as needed, set root password and create Admin user (koha-admin) </li>
  <li>Enable EPEL – sudo yum –y install epel-release</li>
  <li>Update Install – sudo yum -y update</li>
  <li>Install Ansible and MySQL Python - sudo yum –y install ansible MySQL-python git cpanminus</li>
  <li>Clone or Download ansible playbook</li>
  <li>Go to Download Location of ansible playbook (~/koha-ansible/mbed-koha)</li>
  <li>Run Ansible - sudo ansible-playbook koha.yml –u root –i inventory.ini –-connection local</li>
  <li>Secure MySQL Database - sudo mysql_secure_installation</li>
</ol>
