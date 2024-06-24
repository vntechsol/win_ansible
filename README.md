Ansible for Windows target machine will relies on WINRM or SSH. There is a Windows SSH but required a bit of works to get the SSHD running on each target machine. Tries to use WINRM where is possible which save lots of hassle.

For anyone who interests in discovering a bit about Ansible configuration management tool for Windows. Suggest to setup a Windows machine using VirtualBox or VMWare WorkStation, etc first. Collects an IP address or DNS name.

You can use one of mine ansible modules for Windows and for example 

git clone https://github.com/vntechsol/win_ansible.git

cd winansible

Edit inventory file and enter an IP address, Windows ansible admin user with password. Remember to keep the password within your environment, as this is an example for you to see only rather than exposing it to public.

Attempt to run the following

ansible-play -i inventory winansible.yml -vvv
