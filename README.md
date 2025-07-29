# 🚀 Proyecto InnovaSys – Automatización con Ansible

## 📌 Descripción

Este proyecto automatiza la configuración de un servidor Ubuntu 24.04 que cumple funciones de portal web (servidor Apache) y servidor de archivos compartidos (Samba), utilizando Ansible.

## 🔧 Requisitos

- Ansible instalado en la máquina de control  
- Acceso SSH funcional al servidor gestionado  
- Python instalado en el nodo gestionado

## 🚀 Ejecución

1. Clonar el repositorio:  
   `git clone https://github.com/usuario/proyecto-innovasys.git`  
   `cd proyecto-innovasys`

2. Verificar y editar IP en `inventory/hosts` si es necesario.

3. Ejecutar el playbook:  
   `ansible-playbook -i inventory/hosts playbook.yml`

## ⚙️ Roles incluidos

- apache: servidor web  
- samba: servidor de archivos compartidos
