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

# Creación de un Repositorio y Primeros Comandos

## Configuración de la Rama por Defecto

A partir de Git 2.28, puedes configurar el nombre de la rama por defecto. El nombre tradicional es `master`, pero es común cambiarlo a `main`.

```bash
git config --global init.defaultBranch main
```

Si ya tienes una rama `master` y quieres cambiarla a `main`:

```bash
git branch -m master main
```

## Creación de un Nuevo Repositorio

```bash
mkdir nombre-del-proyecto
cd nombre-del-proyecto
git init
```

Esto crea un repositorio Git vacío en el directorio especificado.

## Zonas o Estados de un Fichero en Git

- **Working Area**: Área de trabajo local donde se realizan cambios.
- **Staging Area**: Zona de preparación donde se colocan los archivos listos para el commit.
- **Local Repository**: Almacena los commits realizados localmente.
- **Remote Repository**: Almacena los commits en un servidor remoto.

## Comandos Básicos

### `git status`
Muestra el estado de los archivos en el área de trabajo y staging.

```bash
git status
```

### `git add`
Agrega archivos a la zona de staging.

```bash
git add archivo.txt
git add .
```

### `git commit`
Guarda los cambios en el repositorio local.

```bash
git commit -m "Mensaje descriptivo del cambio"
```

### `git log`
Muestra el historial de commits.

```bash
git log
git log --oneline
```

### `git diff`
Compara cambios entre commits, ramas, etc.

```bash
git diff
```

**Ejemplo de flujo de trabajo básico:**

1. Hacer cambios en los archivos.
2. Añadir los cambios al staging area.
   ```bash
   git add .
   ```
3. Hacer un commit con una descripción de los cambios.
   ```bash
   git commit -m "Descripción de los cambios"
   ```

