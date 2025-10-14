Proyecto de ejemplo: Simpsons API

Este repositorio contiene un pequeño proyecto en TypeScript/HTML que consume la The Simpsons API.

Pasos para subir el proyecto a GitHub (PowerShell)

1) Configurar Git (si no lo hiciste aún)

```powershell
git config --global user.name "Tu Nombre"
git config --global user.email "tu@correo.com"
```

2) Inicializar el repositorio local, añadir archivos y crear el primer commit

```powershell
cd "z:\GITREPO\TPprog3\facultadTPs\TypeScript\tp1"
git init
git add .
git commit -m "Initial commit"
```

3) Crear el repo remoto en GitHub

- Opción A (interfaz web):
  - Ve a https://github.com/new, pon el nombre del repo (por ejemplo `simpsons-api`), crea el repo y copia la URL remota HTTPS.

- Opción B (gh CLI, si tienes instalada la CLI y estás autenticado):

```powershell
# Reemplaza <OWNER>/<REPO> por tu usuario y nombre de repo
gh repo create <OWNER>/<REPO> --public --source=. --remote=origin --push
```

4) Añadir el remoto y subir (si creaste el repo via web)

```powershell
# Reemplaza <URL_REMOTE> por la URL que te dio GitHub, p. ej. https://github.com/tuUsuario/simpsons-api.git
git remote add origin <URL_REMOTE>
git branch -M main
git push -u origin main
```

Comandos útiles

```powershell
git status
git log --oneline
git remote -v
```

Notas y recomendaciones

- He creado un `.gitignore` que excluye `node_modules/` y `dist/` entre otros; ajústalo si necesitas incluir algún archivo de build.
- Si quieres, puedo ejecutar los comandos git aquí (inicializar, commit y push) si me das permiso para correrlos en tu entorno. También puedo ayudarte a crear el repo en GitHub con el gh CLI si lo tienes instalado y autenticado.
