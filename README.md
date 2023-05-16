# ansible-k8-cluster
X Node k8 Cluster Config Using Ansible Playbook :)



steps :

$hostnamectl
$ifconfig
cat /etc/hosts
ip hostname
$cp env_variables playbook/


setip :

ansible playbook settingup_kubernetes_cluster.yml


$kubectl get nodes

$ansible playbook join------




tasks 
  tasks:
    - name: Install necessary packages
      yum:
        name: "{{ item }}"
        state: present
      with_items:
        - yum-utils
        - device-mapper-persistent-data
        - lvm2

