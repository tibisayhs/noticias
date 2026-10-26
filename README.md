# Radar IA & Negocios

Boletín de noticias de inteligencia artificial de Tiby Hernández, para marcas personales y empresas.

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub y sube estos archivos: `index.html`, `.nojekyll` y `README.md`.
2. Ve a Settings > Pages. En "Build and deployment" elige "Deploy from a branch", rama `main`, carpeta `/ (root)`.
3. Espera uno o dos minutos. Tu enlace será `https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/`.

Los enlaces para compartir por WhatsApp se generan solos con esa dirección. Si usas un dominio propio, funcionan igual.

## Cómo editar el contenido
En GitHub, el panel de administración no está disponible (ese panel funciona solo dentro de Claude). Las ediciones viven en `index.html`, dentro de la etiqueta:

    <script id="data" type="application/json"> ... </script>

Ahí está la lista `editions`. Cada edición tiene `id`, `fecha`, `estado` ("publicada" o "borrador"), `titulo`, `intro`, `noticias`, `mirada` y `reto`. Para publicar una edición nueva, copia una existente, cambia sus textos, su `id` y su `fecha`, y pon `"estado": "publicada"`. La portada muestra siempre la más reciente. Edita con cuidado: respeta las comillas y las comas.

Para eliminar las ediciones de ejemplo, borra las que tienen `"demo": true`.

## Notas importantes
- Las fuentes Scholar Italic y Scholar Bold Italic están incrustadas en `index.html`. Verifica que tu licencia permita su uso en web antes de publicar.
- La vista previa de WhatsApp (Open Graph) es la misma para todos los enlaces, porque es una sola página. Para que cada edición tenga su propia tarjeta hace falta un servidor.
- El reto del día guarda la respuesta solo en el dispositivo del lector.
