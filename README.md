# Proyecto fin de curso 2º de ASIR - Gestión de creación de infraestrucutra, configuración y administración de software con AWX

## Índice

- [](#)

# PROYECTOAWX

## Inicio

* Creamos entorno de trabajo
```
PROJECT_NAME="proyecto"
PROJECT_DIR="${HOME}/${PROJECT_NAME}"
mkdir -p $PROJECT_DIR

PROJECT_REPO_NAME="proyectoawx"
PROJECT_REPO_URL="https://github.com/jpcarmona/proyectoawx.git"
git clone $PROJECT_REPO_URL ${PROJECT_DIR}/${PROJECT_REPO_NAME}
```

* Volúmenes permanete para AWX
```
sudo mkdir -p /var/lib/awx/
sudo chown -R $USER. /var/lib/awx/
```

* Despliegue AWX
```
cd ${PROJECT_DIR}/${PROJECT_REPO_NAME}/awxcompose
docker-compose up -d
```

* Creación de entorno virtual de python
```
sudo apt install python3-venv

python3 -m venv ${PROJECT_DIR}/entorno
source ${PROJECT_DIR}/entorno/bin/activate

pip install -r ${PROJECT_DIR}/${PROJECT_REPO_NAME}/requeriments.txt
```

* Variables para API AWX
```
## For all connections:
AWXUSER="awxuser"
AWXPASS="awxpass"
AWXHOST="http://localhost"
## For naming resources:
PROJECT_NAME="proyecto"
PROJECT_ORG="Default"
## For projects:
PROJECT_URL="git@github.com:jpcarmona/proyectoawx.git"
PROJECT_BRANCH="master"
##For credentials:
SSH_KEY_FILE="${HOME}/.ssh/id_rsa"

# Variables de plantillas de trabajo de AWX
## Playbook:
PLAYBOOK_FILE="playbooks/create_servers.yml"
## Inventory:
INVENTORY_FILE="inventories/local.yml"
```

