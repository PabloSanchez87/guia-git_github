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

# Instalación y Configuración de Git

## ¿Qué es Git?

Git es un sistema de control de versiones distribuido, que permite gestionar el historial de cambios de un proyecto. Es rápido, escalable y permite a múltiples desarrolladores trabajar en paralelo.

### Características de Git
- **Control de versiones eficiente**: Facilita el seguimiento de cambios y permite revertir a versiones anteriores.
- **Trabajo en paralelo**: Los desarrolladores pueden trabajar en diferentes ramas sin interferencias.
- **Descentralización**: Cada desarrollador tiene una copia completa del repositorio.
- **Rápido y ligero**: Optimizado para manejar grandes volúmenes de datos.
- **Seguridad**: Uso de SHA-1 para asegurar la integridad del código.

## ¿Qué es GitHub?

GitHub es una plataforma de desarrollo colaborativo basada en Git, que permite a los desarrolladores alojar sus repositorios, colaborar con otros y gestionar proyectos.

### Funcionalidades de GitHub
- **Colaboración facilitada**: Contribuciones, revisiones y discusiones.
- **Control de versiones**: Seguimiento y gestión de diferentes versiones de un proyecto.
- **Integración continua (CI/CD)**: Automatización de pruebas y despliegue.
- **Documentación y gestión de proyectos**: Herramientas para organizar tareas y documentar el proyecto.

## Instalación de Git

### Windows
1. Descargar Git desde [git-scm.com](https://git-scm.com/).
2. Ejecutar el instalador y seguir las instrucciones.

### macOS
```bash
brew install git
```

### Linux
```bash
sudo apt-get install git
```

## Configuración Inicial

Configura Git con tu nombre y correo electrónico, estos serán utilizados en los commits.

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tuemail@example.com"
git config --global core.editor "code --wait"  # Configura Visual Studio Code como editor
```

Para verificar la configuración:

```bash
git config --list
```

## Manejo de Saltos de Línea

### Diferencias entre sistemas operativos
- **Windows**: Utiliza CRLF.
- **macOS/Linux**: Utiliza LF.

Configura Git para manejar correctamente los saltos de línea según tu sistema operativo:

```bash
# Windows
git config --global core.autocrlf true

# macOS/Linux
git config --global core.autocrlf input
```

[Documentación oficial de Git sobre manejo de saltos de línea](https://docs.github.com/es/get-started/getting-started-with-git/configuring-git-to-handle-line-endings?platform=mac)
