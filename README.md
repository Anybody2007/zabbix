# ZABBIX deploy in a simple Docker Configuration

This repository contains a Docker Compose setup for running a Zabbix server, alongside the necessary enviroment configuration files for security. It is designed to be easily customizable and deployable.

You can use this ZABBIX server for your small/medium office, so that you can manage your office systems from a central location.

## Contents

- `docker-compose.yml`: Docker Compose file to set up the Bind9 DNS server.
- `.env`: Containg all the customizable variables.

## Quick Start

1. **Clone the Repository**

   Clone this repository to your local machine to get started.

   ```bash
   git clone https://github.com/Anybody2007/zabbix.git
   ```

2. **Configure ZABBIX deployment via env**

    Suggestion - It's better to use a `.env` file, because you can maintain the security and best practice.

    Update `.env` as per your requirements. Like changing the `mysql` `root` account `password` and other `password`.

    - `MYSQL_ROOT_PWD=zabbix123` you can change in the env file
    - `ZABBIX_VERSION=trunk-centos` you can change the tag to `trunk-ubuntu` or `trunk-alpine`

         For more details of the other image tags checkout the links - https://hub.docker.com/u/zabbix https://www.zabbix.com/container_images
    - TIME_ZONE="Asia/Kolkata" change the time zone as per your requirment
    - MYSQL_USR="root" I have chose the user root because 

