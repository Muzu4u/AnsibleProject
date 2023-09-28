# AnsibleProject
Ansible Playbook to serve simple Laravel project via Nginx Server. 
For CI/CD we have used GitHub Actions to trigger builds on master branch upon every push.

To run this playbook use following command: ansible-playbook playbook.yaml
Ansible Playbook Algorithm
1) Install all dependencies (Nodejs, Composer, Nginx, PHP)
2) created a Folder
3) In that folder created laravel project using composer
4) Installed dependencies required to run laravel project
5) Given permission to nginx for laravel project to run
6) Copied laravel config file to /etc/nginx/sites-available
7) Restart Nginx
