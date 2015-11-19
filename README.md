# nginx-modsec

This project deploys via Vagrant/Ansible a CentOS 6 server with nginx and ModSecurity. Its purpose is analyzing the cause of issue https://github.com/SpiderLabs/ModSecurity/issues/977

First, dependencies for building the software are installed. Then source code is downloaded, a patch is applied to fix the issue, and the binaries are built. The directories used
for config files and binaries are "Red Hat style" (/usr/sbin/nginx for the binaries, /etc/nginx/nginx.conf for configuration and so on) like a RPM package would do. An init script
for nginx service is also included.


