# 🚀 Proyecto InnovaSys – Automatización con Ansible

## 📌 Descripción

Este proyecto automatiza la configuración de un servidor Ubuntu 24.04, que cumple funciones de:

- 🕸️ Portal web con Apache
- 📁 Servidor de archivos compartidos mediante Samba

Todo se gestiona desde una máquina de control con Ansible, aplicando buenas prácticas de organización usando roles, handlers, plantillas y variables.

---

## 🔧 Requisitos

- Ansible instalado en la máquina de control
- Conexión SSH funcional al servidor gestionado
- Python instalado en el nodo gestionado (servidor)

---

## 📂 Estructura del Proyecto

   ```text
   innovaSys/
   ├── hosts                 # Inventario con IP o nombre del servidor
   ├── site.yml             # Playbook principal
   ├── roles/               # Roles organizados por servicio
   │   ├── apache/          # Configuración de Apache
   │   │   ├── tasks/
   │   │   ├── templates/
   │   │   └── handlers/
   │   └── samba/           # Configuración de Samba
   │       ├── tasks/
   │       └── handlers/

---

## 🚀 Ejecución del Playbook

1. Clona el repositorio:

   ```bash
   git clone https://github.com/usuario/proyecto-innovasys.git
   cd proyecto-innovasys

2. Abre el archivo hosts y edita la IP o nombre del servidor si es necesario.

3. Ejecuta el playbook principal:
   ```bash
   ansible-playbook -i hosts site
   
## ⚙️ Roles incluidos
apache: Encargado de instalar y configurar el servidor web Apache, incluyendo su página personalizada.

samba: Configura un servidor de archivos compartidos con autenticación.

## 🧪 Verificación
Acceso web: Desde un navegador web usando la IP del servidor.

Carpeta compartida: Desde un cliente Linux (por ejemplo, Linux Lite) accediendo a través de la red.
