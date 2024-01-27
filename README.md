# infrastructure-as-code
Aplicación de Código de Infraestructura

## Preparacion de Entorno

```sh
python3 -m venv /opt/ansible
```

```sh
ENTORNO=dev ansible-playbook -i $ENTORNO 01.install.yaml
```

# Provisionamiento de Entorno Parametria

```sh
ENTORNO=dev
ansible-playbook -i $ENTORNO 03.consul.yaml
ansible-playbook -i $ENTORNO 02.vault.yaml
```
