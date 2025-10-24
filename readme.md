# Bootcamp Git - Documentación

## Descripción

Este proyecto forma parte del bootcamp de Git, diseñado para aprender los conceptos fundamentales y comandos esenciales de Git para el control de versiones.

## Objetivos de Aprendizaje

- Comprender los conceptos básicos de Git
- Aprender los comandos fundamentales
- Practicar flujos de trabajo con Git
- Manejar branches y merges
- Colaborar usando repositorios remotos

## Estructura del Proyecto

```
bootcamp-git/
├── document.md          # Este archivo de documentación
├── src/                 # Código fuente (si aplica)
├── exercises/           # Ejercicios prácticos
└── README.md           # Información general del proyecto
```

## Comandos Git Básicos

### Configuración Inicial
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu.email@ejemplo.com"
```

### Comandos Fundamentales
```bash
# Inicializar un repositorio
git init

# Clonar un repositorio
git clone <url-del-repositorio>

# Ver el estado del repositorio
git status

# Agregar archivos al staging area
git add <archivo>
git add .  # Agregar todos los archivos

# Hacer commit
git commit -m "Mensaje descriptivo del commit"

# Ver historial de commits
git log
git log --oneline  # Versión resumida
```

### Trabajo con Branches
```bash
# Crear una nueva branch
git branch <nombre-branch>

# Cambiar a una branch
git checkout <nombre-branch>

# Crear y cambiar a una nueva branch
git checkout -b <nombre-branch>

# Listar branches
git branch

# Mergear una branch
git merge <nombre-branch>

# Eliminar una branch
git branch -d <nombre-branch>
```

### Repositorios Remotos
```bash
# Agregar un repositorio remoto
git remote add origin <url-del-repositorio>

# Ver repositorios remotos
git remote -v

# Subir cambios al repositorio remoto
git push origin <nombre-branch>

# Descargar cambios del repositorio remoto
git pull origin <nombre-branch>

# Fetch (descargar sin mergear)
git fetch origin
```

## Flujo de Trabajo Recomendado

1. **Planificación**: Identificar qué cambios se van a realizar
2. **Branch**: Crear una nueva branch para la funcionalidad
3. **Desarrollo**: Realizar los cambios necesarios
4. **Staging**: Agregar archivos modificados al staging area
5. **Commit**: Hacer commit con un mensaje descriptivo
6. **Push**: Subir los cambios al repositorio remoto
7. **Pull Request/Merge Request**: Solicitar revisión e integración
8. **Merge**: Integrar los cambios a la branch principal

## Buenas Prácticas

### Mensajes de Commit
- Usar el imperativo: "Agrega funcionalidad" en lugar de "Agregando funcionalidad"
- Ser descriptivo pero conciso
- Usar prefijos cuando sea apropiado:
  - `feat:` para nuevas funcionalidades
  - `fix:` para corrección de bugs
  - `docs:` para documentación
  - `style:` para cambios de formato
  - `refactor:` para refactoring de código

### Organización de Branches
- `main/master`: Branch principal, siempre estable
- `develop`: Branch de desarrollo
- `feature/nombre-funcionalidad`: Para nuevas funcionalidades
- `hotfix/nombre-fix`: Para correcciones urgentes

## Ejercicios Prácticos

### Ejercicio 1: Configuración Inicial
1. Configurar nombre de usuario y email
2. Inicializar un repositorio
3. Crear un archivo README.md
4. Hacer el primer commit

### Ejercicio 2: Trabajo con Branches
1. Crear una nueva branch llamada `feature/nueva-funcionalidad`
2. Realizar cambios en la branch
3. Hacer commit de los cambios
4. Mergear la branch a main

### Ejercicio 3: Repositorio Remoto
1. Crear un repositorio en GitHub/GitLab
2. Conectar el repositorio local con el remoto
3. Subir los cambios al repositorio remoto
4. Clonar el repositorio en otra ubicación

## Recursos Adicionales

- [Documentación Oficial de Git](https://git-scm.com/doc)
- [Pro Git Book](https://git-scm.com/book)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)
- [Visualizing Git](https://git-school.github.io/visualizing-git/)

## Solución de Problemas Comunes

### Error: "fatal: not a git repository"
**Solución**: Asegúrate de estar en un directorio que sea un repositorio Git o inicializa uno con `git init`.

### Error: "Your branch is ahead of 'origin/main'"
**Solución**: Usa `git push origin main` para subir tus commits locales al repositorio remoto.

### Error: "merge conflict"
**Solución**: 
1. Abre los archivos en conflicto
2. Resuelve los conflictos manualmente
3. Usa `git add` para marcar como resuelto
4. Haz `git commit` para finalizar el merge

## Contribuciones

Si encuentras errores en esta documentación o tienes sugerencias de mejora:

1. Haz un fork del repositorio
2. Crea una branch para tus cambios
3. Realiza las modificaciones
4. Envía un pull request

## Contacto

Para preguntas o dudas sobre este bootcamp, puedes contactar a:
- Email: instructor@bootcamp.com
- Slack: #bootcamp-git

---

*Última actualización: 24 de octubre de 2025*