# events-landing
Commercial site for event planners and organizers.

# [NOMBRE DE LA MARCA] · Landing

Sitio comercial para planners y organizadores de eventos. Presenta la plataforma de listas de regalos con reservas, lista de agradecimientos y hasta 10 listas por evento.

Estado: **acceso anticipado.** La landing no promete funciones que aún no estén terminadas.

## Archivos

```
landing-planner/
├── index.html   # Landing completa: diseño, secciones y contacto
└── README.md    # Este archivo
```

## Publicar en GitHub Pages

1. Crea un repositorio público, por ejemplo `landing-planner`.
2. Sube `index.html` y `README.md` a la rama `main`.
3. Ve a **Settings → Pages**, elige **Deploy from a branch**, rama `main`, carpeta `/ (root)`.
4. El sitio quedará en `https://tu-usuario.github.io/landing-planner/`.

## Antes de publicar: completar los datos

Busca estos marcadores en `index.html` (Ctrl + F) y reemplázalos:

| Marcador | Dónde aparece | Qué poner |
|---|---|---|
| `[NOMBRE DE LA MARCA]` | título, menú, pie de página | Nombre comercial definitivo |
| `[PRECIO]` (3 veces) | sección de precios | Precio por evento de cada plan |
| `[CORREO DE CONTACTO]` | botón de correo | Correo para solicitudes |
| `50761300188` | botón de WhatsApp | Confirmar que es el número de contacto comercial |

Revisa también:

- **Aviso de privacidad y términos de uso.** Los enlaces del pie apuntan a `#`. Antes de cobrar, deben existir las páginas reales.
- **Texto de Amazon.** El pie de página aclara que no hay afiliación. Mantenlo.
- **Vista previa del panel.** Es una ilustración, no una captura real. Reemplázala cuando el panel esté conectado a Firebase.

## Qué no debe cambiar sin revisar

- **Promesas.** Cada función que aparece en la landing debe estar disponible en el producto antes de cobrarla. Si una función se retrasa, quítala del texto.
- **Confirmación de compra.** La landing dice que Amazon no informa las compras. Si en el futuro se obtiene esa información por otro medio, actualiza la pregunta frecuente.
- **Precios.** Son marcadores. No publiques cifras sin validarlas con clientes reales.

## Hoja de ruta de la landing

1. Completar datos y publicar la versión de acceso anticipado.
2. Agregar una captura real del panel del planner cuando esté conectado a Firebase.
3. Crear las páginas de aviso de privacidad y términos.
4. Agregar un formulario de solicitud con registro de cada prospecto, por ejemplo con Google Forms o un servicio gratuito.
5. Medir de dónde llegan las solicitudes y ajustar el mensaje.

## Licencia

Uso comercial de la marca reservado a su titular. Los nombres y logotipos de terceros (Amazon, WhatsApp, Google) pertenecen a sus respectivos dueños.
