# vibacs-assets

Repositorio de assets estáticos del proyecto **VIBACS** (Vigilància a Barcelona del canvi climàtic i l'impacte sobre la salut) de la [Agència de Salut Pública de Barcelona (ASPB)](https://www.aspb.cat/).

## Para qué sirve

Las páginas interiores del portal VIBACS son aplicaciones Shiny (`.qmd`). Shiny Server solo sirve la aplicación R, no archivos sueltos como imágenes o SVGs, así que los logos e iconos no pueden referenciarse con rutas relativas locales.

Este repositorio resuelve eso: los archivos se publican aquí y se consumen desde URLs de GitHub, accesibles desde cualquier entorno (Shiny Server, shinyapps.io, local).

Para usarlo, reemplazá las rutas locales de los assets en los HTML embebidos dentro de los `.qmd` por URLs a este repositorio:

```
assets/logos/aspb-logo-header.svg
→ https://raw.githubusercontent.com/jcorvetto1974/vibacs-assets/main/logos/aspb-logo-header.svg
```

## URL base

```
https://raw.githubusercontent.com/jcorvetto1974/vibacs-assets/main/
```

## Estructura

```
vibacs-assets/
├── logos/                        ← Logos institucionales
│   ├── aspb-logo-header.svg      ← Logo ASPB header (desktop)
│   ├── aspb-logo-footer.svg      ← Logo ASPB footer
│   ├── aspb-brand-mark.svg       ← Marca ASPB (header mobile sticky)
│   ├── vibacs-logo.svg           ← Logo VIBACS completo (desktop)
│   └── vibacs-logo-mobile.svg    ← Logo VIBACS reducido (mobile)
│
├── icons/                        ← Iconos de interfaz y temáticas
│   ├── icon-pe.svg               ← Pobresa energètica
│   ├── icon-calor.svg            ← Temperatura
│   ├── icon-aire.svg             ← Qualitat de l'aire
│   ├── icon-aigua.svg            ← Disponibilitat i qualitat de l'aigua
│   ├── icon-mob.svg              ← Mobilitat
│   ├── icon-al.svg               ← Alimentació
│   ├── icon-vectors.svg          ← Vectors
│   ├── arrow-right.svg           ← Flecha tiles portal
│   ├── arrow-right-white.svg     ← Flecha tiles (variante blanca)
│   ├── favicon.svg
│   ├── apple-touch-icon.png
│   ├── icon-192.png
│   └── icon-512.png
│
├── tiles/                        ← Fotos de fondo de los tiles del portal
│   ├── tile-pe.jpg
│   ├── tile-calor.jpg
│   ├── tile-aire.jpg
│   ├── tile-aigua.jpg
│   ├── tile-mob.jpg
│   ├── tile-al.jpg
│   └── tile-vectors.jpg
│
├── hero/                         ← Assets del hero del portal
│   └── v-symbol.svg
│
└── extras/                       ← Assets auxiliares (overlays, decoración)
    ├── arrow-right-aigua-dup.svg
    ├── arrow-right-aire-dup.svg
    ├── arrow-right-alimentacio-dup.svg
    ├── arrow-right-calor-dup.svg
    ├── arrow-right-movilitat-dup.svg
    ├── arrow-right-vectors-dup.svg
    ├── calor-banda-label-multiply.svg
    ├── calor-fondo-multiply.svg
    ├── header-linea-superior.svg
    └── header-linea-vertical.svg
```
