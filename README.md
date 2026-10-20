# 🤝 Fernanda — Landing de consultora freelance en RRHH

Landing page de **una consultora independiente en Recursos Humanos**: Fernanda, que trabaja como **freelance** (una sola persona, no una consultora ni una empresa). Por eso todo el texto está redactado en **primera persona del singular** ("Sobre mí", "Mi enfoque", "Trabajo con…"), nunca en plural.

La página reúne su propuesta de valor, los servicios que ofrece, su forma de trabajar, una presentación personal y un formulario de contacto.

## Secciones

| # | Sección | id | Qué contiene |
|---|---------|----|--------------|
| 1 | Header | — | Nombre de la consultora + navegación anclada a cada sección |
| 2 | Inicio | `#inicio` | Propuesta de valor en primera persona y botones de acción |
| 3 | Servicios | `#servicios` | 6 servicios en tarjetas: qué es y para quién sirve cada uno |
| 4 | Trabajemos juntas | `#como-trabajo` | Proceso de trabajo en 3 pasos: diagnóstico, propuesta y acompañamiento |
| 5 | Sobre mí | `#sobre-mi` | Presentación personal + ilustración |
| 6 | Contacto | `#contacto` | Formulario + datos de contacto |
| 7 | Footer | — | Nombre, copyright y enlace para volver al inicio |

## Servicios

1. Reclutamiento y selección
2. Capacitación y desarrollo
3. Consultoría y auditoría de RRHH
4. Gestión de nómina y liquidación de sueldos
5. Cultura organizacional y clima laboral
6. Evaluación de desempeño

Cada tarjeta explica **qué es** el servicio y **para quién** sirve.

## Características

- HTML semántico (`header`, `nav`, `main`, `section`, `article`, `footer`) y accesible: `label for` + `id` en todos los campos, `alt` en la imagen, enlace "saltar al contenido" y foco visible con teclado.
- `<head>` completo con SEO y Open Graph (`og:locale` `es_AR`).
- Diseño responsive (una sola columna en pantallas angostas), limpio y corporativo pero cercano.
- Estilos en un archivo aparte (`style.css`), con la misma paleta original: verde azulado `#00796b`, verde oscuro `#004d40`, grises y fondo `#f9f9fb`.
- Sin dependencias ni build: se abre directamente en el navegador.

## ⚠️ Configurar ANTES de publicar

Ninguno de estos pasos está hecho a propósito: **no se inventan datos** (ni teléfono, ni mail, ni clientes, ni cifras). Todo lo que falta está marcado como `[a completar]` o con un placeholder.

1. **Formspree (obligatorio para que el formulario funcione).**
   El `<form>` de `index.html` tiene `method="POST"` y apunta a:

   ```html
   <form action="https://formspree.io/f/REEMPLAZAR_POR_EL_ID_REAL" method="POST">
   ```

   `REEMPLAZAR_POR_EL_ID_REAL` es un **placeholder**: hay que crear el formulario en [formspree.io](https://formspree.io), copiar el ID real y reemplazarlo en esa línea (está marcado con un comentario `⚠ CONFIGURAR ANTES DE PUBLICAR` en el HTML).

   > **Hasta que se reemplace ese ID, el formulario NO envía nada**: al enviarlo el mensaje se pierde.

2. **Nombre de la consultora.** La landing usa **"Fernanda"** (nombre del proyecto). Si la clienta se llama diferente, cambiar el `<h1>` del header, el `<title>`, las meta etiquetas (`description`, `og:title`, `og:description`, `og:site_name`), el `_subject` del formulario y el footer.

3. **Datos de contacto.** En la sección `#contacto` hay una lista con `[a completar]`: correo electrónico, WhatsApp, LinkedIn y ubicación/modalidad de trabajo. Reemplazar por los datos reales (borrando la clase `pendiente` para que dejen de verse en cursiva gris).

4. **Open Graph.** Descomentar y completar `og:url` y `og:image` en el `<head>` con la URL definitiva del sitio y la imagen de previsualización (JPG/PNG de al menos 1200x630 px).

5. **Imagen de la sección "Sobre mí".** Hoy es una ilustración decorativa (`img/consultora-rrhh.svg`). Si hay una foto real de la consultora, reemplazar el archivo y ajustar el atributo `alt`.

## Cómo usarlo

1. Descargá el repositorio.
2. Abrí `index.html` en tu navegador.
3. Para adaptarlo, editá los textos de `index.html` y, si hace falta, los colores de `style.css`.

## Estructura

```
05-fernanda/
├── index.html              ← página principal
├── style.css               ← estilos (reglas originales + bloque "AGREGADOS" al final)
├── index.comentado.html    ← copia del index.html explicada línea por línea
├── style.comentado.css     ← copia del style.css explicada regla por regla
├── img/
│   └── consultora-rrhh.svg ← ilustración de la sección "Sobre mí"
└── README.md
```

Los archivos `.comentado` son material de estudio: son copias **exactas** de los originales (cero cambios funcionales) con comentarios en español.

## Demo

🌐 [https://cuutii.github.io/Fernanda/](https://cuutii.github.io/Fernanda/)

## Tecnologías

- HTML5
- CSS3

## Autor

**Maximo Sanabria** — GitHub [@cuutii](https://github.com/cuutii) — [LinkedIn](https://www.linkedin.com/in/maximo-sanabria-cutib/)
