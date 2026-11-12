# Huellas de Esperanza – Actividad Autónoma #3

Prototipo estructural de un sistema web de control de rescate y adopción animal.
Desarrollado con HTML5 semántico, sin CSS, JavaScript, servidor ni base de datos,
de acuerdo con la guía de la Unidad 2.

## Archivos principales

- `index.html`: panel principal y resumen del refugio.
- `reportar.html`: formulario de captura de un nuevo rescate.
- `rescates.html`: tabla de casos de demostración.
- `assets/img/`: carpeta prevista para recursos gráficos.
- `docs/Informe_Actividad_3_DSI.pdf`: informe académico.
- `docs/evidencias/`: capturas del navegador y vistas del código fuente.

## Ejecución en Visual Studio Code

1. Descomprima el proyecto.
2. Abra la carpeta `Proyecto_DSI_Rescate_Animal` en Visual Studio Code.
3. Abra `index.html` con un navegador o con la extensión Live Server.
4. Utilice el menú de navegación para acceder a las otras dos páginas.

## Alcance del formulario

El formulario emplea validaciones nativas de HTML5 y el método GET para enviar
los campos a `rescates.html`. Como esta actividad solicita únicamente el prototipo
estructural HTML5, no existe almacenamiento persistente ni actualización automática
de la tabla. Los tres registros visibles son datos ficticios de demostración.

## Gitflow solicitado

El repositorio remoto debe crearse en GitHub con el nombre sugerido:
`proyecto-dsi-huellas-de-esperanza`.

Una vez creado el repositorio vacío en GitHub, abra la terminal de VS Code en esta
carpeta y ejecute los comandos siguientes, sustituyendo `TU_USUARIO` por su usuario
real de GitHub:

```bash
git init
git add .
git commit -m "chore: crear estructura inicial del proyecto"
git branch -M master
git branch develop
git switch develop
git switch -c feature/maquetacion-html
git add .
git commit -m "feat: maquetar paginas HTML5 semanticas"
git switch develop
git merge --no-ff feature/maquetacion-html -m "merge: integrar maquetacion HTML5"
git remote add origin https://github.com/TU_USUARIO/proyecto-dsi-huellas-de-esperanza.git
git push -u origin master
git push -u origin develop
git push -u origin feature/maquetacion-html
```

Para evidenciar las ramas y las fusiones:

```bash
git branch -a
git log --graph --oneline --decorate --all
```

## Validación HTML5

La revisión estructural local no sustituye la validación oficial. Para completar este
requisito, cargue individualmente `index.html`, `reportar.html` y `rescates.html` en
el Markup Validation Service de W3C: https://validator.w3.org/

Guarde una captura de cada resultado de validación y agréguela a `docs/evidencias/`.
