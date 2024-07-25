## Contenidos

1. [**Instalación y Configuracion Git**](1-Instalacion_y_Configuracion_Git.md)
2. [**Creación de Repositorio y Primeros Comandos**](2-Creacion_de_Repositorio_y_Primeros_Comandos.md)
3. [**Ramas, Staging y git Log**](3-Ramas_Staging_y_Git_Log.md)
4. [**Manejo de Ramas y Ejemplo**](4-Manejo_de_Ramas_y_Ejemplo.md)
5. [**Gitignore Stash y Clonacion**](5-Gitignore_Stash_y_Clonacion.md)
6. [**Primer Repositorio en GitHub**](6-Primer_Repositorio_en_GitHub.md)
7. [**Publicación y Personalización en GitHub**](7-Publicacion_y_Personalizacion_en_GitHub.md)
8. [**CheatSheet Comandos Git y GitHub**](CheatSheet_Comandos_Git_y_GitHub.md)

---

# Nuestro Primer Repositorio en GitHub

## Creación de un Repositorio en GitHub

1. Inicia sesión en [GitHub](https://github.com/).
2. Haz clic en "New" para crear un nuevo repositorio.
3. Rellena los detalles del repositorio (nombre, descripción, visibilidad).
4. Selecciona "Initialize this repository with a README" para crear un archivo README.md por defecto.
5. Haz clic en "Create repository".

## Clone vs. Fork

- **Clone**: Copia exacta de un repositorio en tu máquina local. Puedes trabajar en él y enviar cambios a un repositorio remoto.
- **Fork**: Crea una copia de un repositorio en tu cuenta de GitHub. Ideal para contribuir a proyectos de otros usuarios.

### Clonar un repositorio
```bash
git clone https://github.com/usuario/repositorio.git
```

### Hacer un fork de un repositorio
1. Ve al repositorio en GitHub que deseas forkear.
2. Haz clic en el botón "Fork" en la esquina superior derecha.
3. Esto creará una copia en tu cuenta de GitHub.

## Colaboración en GitHub

### Pull Requests

Los Pull Requests son una manera de proponer cambios en un repositorio.

1. Haz cambios en una rama de tu fork.
2. Navega al repositorio original y crea un Pull Request comparando tu rama con la rama principal del repositorio original.

### Issues

Los Issues son una herramienta para reportar errores, sugerir mejoras o discutir aspectos del proyecto.

1. Ve a la pestaña "Issues" en el repositorio de GitHub.
2. Haz clic en "New Issue" para crear un nuevo reporte o sugerencia.

**Ejemplo de flujo de trabajo en GitHub:**

1. Haz un fork de un repositorio para contribuir.
2. Clona tu fork a tu máquina local.
3. Crea una nueva rama para tu trabajo.
4. Haz cambios, commits y luego push a tu fork.
5. Crea un Pull Request para fusionar tus cambios en el repositorio original.

