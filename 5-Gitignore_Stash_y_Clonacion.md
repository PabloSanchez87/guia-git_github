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

# Gitignore, Stash y Clonación de Repositorios

## Gitignore
Un archivo `.gitignore` se usa para indicar a Git qué archivos o directorios ignorar.

### Crear un archivo .gitignore
```bash
echo "node_modules/" >> .gitignore
echo "*.log" >> .gitignore
```

### Añadir plantillas a .gitignore
Existen plantillas comunes para diferentes lenguajes y frameworks. 

- Puedes encontrar plantillas en [github.com/github/gitignore](https://github.com/github/gitignore).

O puedes utilizar la herramienta de Toptal para crear archivos .gitignore personalizados según tus necesidades y tecnologías:
- [gitgonre.io](https://www.toptal.com/developers/gitignore/)

## Stash

`git stash` permite guardar cambios no confirmados temporalmente.

### Guardar cambios en el stash
```bash
git stash
```

### Listar elementos en el stash
```bash
git stash list
```

### Aplicar cambios desde el stash
```bash
git stash apply stash@{0}
```

### Eliminar elementos del stash
```bash
git stash drop stash@{0}
```

## Clonación de Repositorios

`git clone` se usa para copiar un repositorio completo a una nueva ubicación.

### Clonar un repositorio
```bash
git clone https://github.com/usuario/repositorio.git
```

### Configurar un repositorio clonado
1. Cambiar al directorio del repositorio clonado.
2. Verificar la configuración de `remote`:
   ```bash
   git remote -v
   ```

**Ejemplo de uso de .gitignore y stash:**

1. Crear un archivo `.gitignore` para evitar incluir archivos innecesarios como `node_modules/` o archivos de configuración local.
2. Utilizar `git stash` para guardar temporalmente el trabajo en progreso cuando necesitas cambiar de contexto sin hacer un commit.
