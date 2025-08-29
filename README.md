# Proyecto InnovaSys - Aprovisionamiento de Servidor con Ansible
## Estudiantes: Alejandro Chambi    -     Melany Lopez

Este proyecto contine un playbook de Ansible para configurar un servidor Ubuntu 24.04 desde cero con dos servicios principales: un servidor web Apache y un servidor de archivos Samba.

# Estructura

El proyecto utiliza roles de Ansibles para una organizacion modular:
- 'roles/apache': Configura el servidor web.
- 'roles/samba': Configura el servidor de archivos.

Las variables globales se gestionan en 'group_vars/all.yml'.

##Como Ejecutar

1. **CLonar el repositorio**
  git clone https://github.com/Alejandro1234/proyecto-innovasys.git
  cd proyecto-innovasys

2. **Configurar el inventario**
   Edita el archivo 'inventory' y reemplaza la IP y el usuario del servidor a gestionar.

3. **Ejecutar el playbook**
   ansible-playbook -i inventory playbook.yml
