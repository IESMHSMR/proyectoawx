# Proyecto fin de curso 2º de ASIR - Gestión de creación de infraestrucutra, configuración y administración de software con AWX

## Índice

- [Introducción](#introducción)
    - [Objetivos de este proyecto](#objetivos-de-este-proyecto)
- [Requisitos](#requisitos)
    - [Tecnologías utilizadas](#tecnologías-utilizadas)
    - [Infraestructura](#infraestructura)
- [¿ Qué es AWX ?](#-qué-es-awx-)

## Introducción

Hablar sobre AWX, Ansible, la automatización de tareas, etc...

### Objetivos de este proyecto



## Requisitos

Para llevar a cabo el funcionamiento de este proyecto se hará uso de distintas tecnologías de sofware libre, se recomendaría tener conocimientos de algunas de estas tecnologías listadas a continuación. Además necesitaremos una infraestructura con OpenStack, en mi caso utilizo la de mi instituto.

### Tecnologías utilizadas

* [Docker](https://docs.docker.com/get-started/) - La versión Community Edition "CE:
```
$ docker --version
Docker version 18.09.6, build 481bc77
```
* [Python3-pip](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/) :
```
$ python3 -m pip --version
pip 19.1.1 from /home/user/.local/lib/python3.6/site-packages/pip (python 3.6)
```
* [Ansible](https://docs.ansible.com/ansible/latest/index.html) :
```
$ ansible --version
ansible 2.8.0
  config file = None
  configured module search path = ['/home/user/.ansible/plugins/modules', '/usr/share/ansible/plugins/modules']
  ansible python module location = /home/user/env/lib/python3.6/site-packages/ansible
  executable location = /home/user/env/bin/ansible
  python version = 3.6.5 (default, Apr  1 2018, 05:46:30) [GCC 7.3.0]
```
* [AWX](https://github.com/ansible/awx)

### Infraestructura

* En nuestro equipo local de desarrollo donde trabajaremos en este proyecto instalaremos la herramienta AWX

* Servidor con Openstack:
Esta herramienta de cloud-computing me la proporcionará mi instituto.

## ¿ Qué es AWX ?