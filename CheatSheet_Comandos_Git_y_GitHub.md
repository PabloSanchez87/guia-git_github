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

# CheatSheet de Comandos Git y GitHub

## Configuración y Ayuda

```bash
# Configurar el nombre de usuario
git config --global user.name "Tu Nombre"

# Configurar el correo electrónico
git config --global user.email "tuemail@example.com"

# Obtener ayuda sobre un comando específico
git help <comando>
```

## Creación de Repositorios

```bash
# Inicializar un nuevo repositorio
git init

# Clonar un repositorio existente
git clone <url>
```

## Realizar Cambios y Commits

```bash
# Añadir un archivo específico al staging area
git add <archivo>

# Añadir todos los archivos al staging area
git add .

# Realizar un commit con un mensaje
git commit -m "mensaje del commit"

# Ver el estado del repositorio
git status

# Mostrar el historial de commits
git log
```

## Trabajar con Ramas

```bash
# Listar todas las ramas
git branch

# Crear una nueva rama
git branch <rama-nueva>

# Cambiar a una rama específica
git checkout <nombre-de-la-rama>

# Crear y cambiar a una nueva rama
git checkout -b <rama-nueva>

# Fusionar una rama en la rama actual
git merge <rama>

# Eliminar una rama
git branch -d <rama>
```

## Trabajo Remoto

```bash
# Añadir un repositorio remoto
git remote add origin <url>

# Enviar cambios al repositorio remoto
git push origin <rama>

# Obtener cambios del repositorio remoto
git fetch

# Obtener y fusionar cambios del repositorio remoto
git pull
```

## Deshacer Cambios

```bash
# Descartar cambios en el directorio de trabajo
git checkout -- <archivo>

# Quitar un archivo del staging area
git reset <archivo>

# Resetear el repositorio al último commit
git reset --hard
```

## Otras Utilidades

```bash
# Guardar cambios no confirmados temporalmente
git stash

# Aplicar cambios guardados en el stash
git stash apply

# Crear una etiqueta (tag) en un commit
git tag <nombre_tag>

# Mostrar detalles de un tag o commit
git show <tag/commit>
```

## Comandos Útiles de GitHub

```bash
# Clonar un repositorio desde GitHub
git clone https://github.com/usuario/repositorio.git
```

## Comandos Avanzados

```bash
# Rebase de una rama sobre otra
git rebase <rama>

# Ver las diferencias entre ramas
git diff <rama1> <rama2>

# Borrar un tag
git tag -d <nombre_tag>

# Listar los remotos configurados
git remote -v

# Renombrar una rama
git branch -m <nombre-nuevo>
```

## Aliases Útiles

```bash
# Crear un alias para un comando frecuente
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.ci commit
git config --global alias.br branch
```

