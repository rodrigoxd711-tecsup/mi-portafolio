# Guia de contribucion

Gracias por tu interés en mejorar este portafolio. Este repositorio reúne la documentación de mis trabajos del curso **Diseño de Interfaces de Programación Avanzado** (Tecsup). Aquí se explica cómo reportar un error, cómo proponer una mejora y qué revisar antes de enviar un Pull Request.

## Tabla de contenidos

- [Antes de empezar](#antes-de-empezar)
- [Como reportar un error](#como-reportar-un-error)
- [Como proponer una mejora](#como-proponer-una-mejora)
- [Convenciones del proyecto](#convenciones-del-proyecto)
- [Checklist del Pull Request](#checklist-del-pull-request)
- [Dudas](#dudas)

## Antes de empezar

- Revisa los [Issues abiertos](https://github.com/rodrigoxd711-tecsup/mi-portafolio/issues) para no duplicar un reporte.
- Necesitas Git, una cuenta de GitHub y un editor con vista previa de Markdown. Se recomienda Visual Studio Code con la extensión **Markdown Preview Mermaid Support**.

## Como reportar un error

Un error es cualquier cosa que no se ve o no funciona como debería: un enlace roto, una imagen que no carga, una tabla que no se renderiza o información incorrecta.

1. Entra a la pestaña **Issues** y haz clic en **New issue**.
2. Escribe un título corto que describa el problema, por ejemplo: `Enlace roto en la guia de Tienda TECSUP`.
3. Completa la descripción con esta plantilla:

```markdown
**Que esperabas que pasara:**
El enlace a la guia abre el archivo docs/GUIA.md.

**Que paso en realidad:**
GitHub muestra el error 404.

**Donde ocurre:**
README.md, seccion "Documentacion del proyecto".

**Captura (opcional):**
Arrastra aqui la imagen.
```

4. Agrega la etiqueta `bug` y envía el Issue.

## Como proponer una mejora

1. Abre primero un Issue con la etiqueta `enhancement` explicando tu idea, para conversarla antes de escribir.
2. Haz un **fork** del repositorio y clónalo:

```bash
git clone https://github.com/TU-USUARIO/mi-portafolio.git
cd mi-portafolio
```

3. Crea una rama con un nombre descriptivo:

```bash
git checkout -b mejora/descripcion-corta
```

4. Haz tus cambios y revísalos en la vista previa.
5. Registra y sube tus cambios:

```bash
git add .
git commit -m "Agrega seccion del laboratorio 06"
git push origin mejora/descripcion-corta
```

6. Abre un **Pull Request** hacia la rama `main` y enlaza el Issue escribiendo `Closes #numero` en la descripción.

## Convenciones del proyecto

| Elemento | Convención | Ejemplo |
|:---------|:-----------|:--------|
| Ramas | `tipo/descripcion-corta` en minúsculas | `fix/enlace-guia` |
| Commits | Verbo en presente, sin punto final | `Corrige enlace a la guia` |
| Títulos del README | Sin tildes, para que las anclas funcionen | `## Instalacion` |
| Imágenes | Carpeta `img/`, en minúsculas y sin espacios | `img/lab05-diagrama.png` |
| Documentos | Carpeta `docs/`, en formato Markdown | `docs/GUIA.md` |

## Checklist del Pull Request

Antes de enviar tu Pull Request, verifica cada punto:

- [ ] El cambio está explicado en la descripción del Pull Request.
- [ ] Revisé la vista previa y todo se renderiza: tablas, listas, código y diagramas.
- [ ] Los enlaces y las imágenes funcionan, incluidos los relativos.
- [ ] Los enlaces de la tabla de contenidos llevan a su sección.
- [ ] Los bloques de código indican su lenguaje (`bash`, `markdown`, etc.).
- [ ] Los mensajes de commit son descriptivos.
- [ ] No incluí contraseñas, tokens ni datos personales.

## Dudas

Si algo no queda claro, abre un Issue con la etiqueta `question` y lo revisamos.