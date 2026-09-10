# Portafolio Académico — Cristhofer Angel Gamero Carrion

Un solo repositorio con las 4 unidades del curso y la página que las muestra.

```
portafolio-cristhofer/
├── index.html        ← la página del portafolio (raíz, para GitHub Pages)
├── foto-perfil.png   ← tu foto de perfil
├── unidad-1/
│   ├── semana-1/
│   ├── semana-2/
│   ├── semana-3/
│   └── semana-4/
├── unidad-2/
│   └── semana-5/ ... semana-8/
├── unidad-3/
│   └── semana-9/ ... semana-12/
└── unidad-4/
    └── semana-13/ ... semana-16/
```

## 1. Crear el repositorio en GitHub

Crea en GitHub un repositorio vacío (sin README) llamado exactamente `BASE-DE-DATOS-II`. Que sea **Público**.

## 2. Subir todo desde VS Code

```bash
cd portafolio-cristhofer
git init
git add .
git commit -m "Primer commit: estructura del portafolio"
git branch -M main
git remote add origin https://github.com/Cristhofer987/BASE-DE-DATOS-II.git
git push -u origin main
```

## 3. Activar GitHub Pages

En el repositorio, ve a `Settings > Pages` → Branch: `main`, carpeta `/ (root)` → Save. En unos minutos tu portafolio estará en `https://Cristhofer987.github.io/BASE-DE-DATOS-II/`.

## 4. La URL ya está puesta en el código

En `index.html`, dentro del bloque `DATOS`, ya está escrita tu URL real:

```js
const REPO_URL = "https://github.com/Cristhofer987/BASE-DE-DATOS-II";
```

No necesitas cambiar nada aquí — solo asegúrate de que el nombre de tu repositorio en GitHub coincida exactamente con `BASE-DE-DATOS-II`.

## 5. Subir un trabajo nuevo cada semana

1. Copia tu archivo dentro de `unidad-N/semana-N/`.
2. `git add . && git commit -m "Semana N: agrego trabajo" && git push`.
3. En `index.html`, dentro del bloque `DATOS`, agrega un objeto en `documentos` de esa semana con `tag`, `titulo`, `descripcion` y `archivo` (ruta exacta, ej: `unidad-2/semana-5/tarea.pdf`).
4. Vuelve a subir el cambio del `index.html` (mismo `git add . && git commit && git push`, o editándolo directo en GitHub.com).
