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

# Ramas, Staging y Git Log

## Creación y Uso de Ramas

Las ramas en Git permiten desarrollar características, corregir errores o experimentar en paralelo sin afectar la rama principal.

### Crear una nueva rama
```bash
git branch nombre-de-la-rama
```

### Cambiar a una rama existente
```bash
git checkout nombre-de-la-rama
```

### Crear y cambiar a una nueva rama
```bash
git checkout -b nombre-de-la-rama
```

### Listar ramas
```bash
git branch
```

### Renombrar una rama
```bash
git branch -m nombre-viejo nombre-nuevo
```

## Staging Area

El área de staging es donde se preparan los cambios antes de hacer un commit.

### Añadir archivos al staging
```bash
git add archivo.txt
git add .
```

### Verificar archivos en staging
```bash
git status
```

### Retirar archivos del staging
```bash
git restore --staged archivo.txt
```

## Git Log

`git log` es una herramienta poderosa para revisar el historial de commits.

### Comando básico
```bash
git log
```

### Formatos de salida
```bash
git log --oneline
git log --graph --oneline
```

### Mostrar detalles de un commit específico
```bash
git show commit-hash
```

**Ejemplo de flujo de trabajo con ramas:**

1. Crear y cambiar a una nueva rama para desarrollar una característica.
   ```bash
   git checkout -b nueva-feature
   ```
2. Hacer cambios y commits en la nueva rama.
3. Volver a la rama principal y fusionar los cambios.
   ```bash
   git checkout main
   git merge nueva-feature
   ```

