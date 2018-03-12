# ansible_restart_worker
An example showing how you can run with ansible-playbook a command to restart a worker on all the available gearman servers.

### Installation
Clone this repository.

### How to run commands
```javascript
cd /INSTALL_DIR
ansible-playbook -i inventories/deploy.yml playbooks/manage_supervisor.yml -e "country_code=ro" -e "service_type=gearman" -e "worker=update_job" -e "worker_action=restart"
```

