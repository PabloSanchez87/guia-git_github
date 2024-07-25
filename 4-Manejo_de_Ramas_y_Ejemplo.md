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

# Manejo de Ramas y Ejercicio Práctico

## Eliminación de Archivos en Git

Para eliminar un archivo y reflejarlo en el historial:

```bash
git rm archivo.txt
git commit -m "Eliminar archivo.txt"
```

Para eliminar un archivo del repositorio pero mantenerlo localmente:

```bash
git rm --cached archivo.txt
```

## Renombrar y Mover Archivos

Git no tiene un comando específico para renombrar archivos, pero puedes usar `git mv` para moverlos y renombrarlos.

```bash
git mv archivo-viejo.txt archivo-nuevo.txt
git commit -m "Renombrar archivo-viejo.txt a archivo-nuevo.txt"
```

## Ejercicio Práctico con Ramas

### Creación de ramas y fusión
1. Crear una nueva rama para una característica:
   ```bash
   git checkout -b feature-x
   ```
2. Realizar cambios y commits en esta rama.
3. Volver a la rama principal y fusionar los cambios:
   ```bash
   git checkout main
   git merge feature-x
   ```

### Manejo de Conflictos de Fusión

Al intentar fusionar ramas, pueden ocurrir conflictos. Para resolverlos:
1. Git mostrará los archivos en conflicto. Abre estos archivos y resuelve los conflictos manualmente.
2. Marca los conflictos como resueltos:
   ```bash
   git add archivo-en-conflicto.txt
   ```
3. Completa el merge:
   ```bash
   git commit
   ```

### Comparación de Ramas

Para ver diferencias entre ramas:
```bash
git diff main..feature-x
```

### Ejemplo de flujo de trabajo:

1. Crear ramas para cada nueva característica o bug.
2. Trabajar en las ramas sin afectar la rama principal.
3. Fusionar cambios una vez que estén listos y probados.
4. Resolver conflictos de manera ordenada.

