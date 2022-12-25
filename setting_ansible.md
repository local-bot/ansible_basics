# ansible basics

### 1 Create and edit inventroy file 
<pre>
for ini format:
touch hosts

for yaml format:
touch hosts.yml
</pre>

## 2\ create configuration file
<pre>
touch ansible.cfg
</pre>

## 3\ example ping module 
<pre>
ansible -i inventory.yaml all -m ping
</pre>

## example package module (apt, yum, dnf...)
<pre>
ansible -i inventory.yaml webservers -m package -a "name=nginx state=present" -b
</pre>