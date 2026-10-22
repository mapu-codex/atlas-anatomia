# Atlas Anatómico 3D — prototipo 0.2

Este prototipo carga el modelo Écorché desde una CDN y usa Three.js para mostrarlo en 3D. Necesita internet para descargar las librerías y el modelo.

## Qué incluye
- Modelo 3D con mallas independientes para huesos y músculos.
- Órbita con mouse o pantalla táctil.
- Selección directa de estructuras y búsqueda por nombre.
- Encendido/apagado de esqueleto, músculos profundos y superficiales.
- Ocultar una estructura, aislarla y controlar la transparencia de los músculos superficiales.
- Preparación inicial para WebXR/VR. No se considera validada hasta probarla en un Quest 3S con una URL HTTPS.

## Cómo abrirlo en Windows (recomendado)
1. Instala Visual Studio Code desde https://code.visualstudio.com/ si aún no lo tienes.
2. Descomprime el archivo ZIP en una carpeta fácil de encontrar, por ejemplo `Documentos\AtlasAnatomico`.
3. Abre Visual Studio Code y elige **Archivo > Abrir carpeta**. Selecciona esa carpeta.
4. En la sección Extensiones, busca e instala **Live Server** (autor Ritwick Dey).
5. Abre `index.html` y pulsa **Go Live** en la esquina inferior derecha.
6. El navegador se abrirá con una dirección local, normalmente `http://127.0.0.1:5500`.
7. Espera a que el modelo se descargue. La primera carga puede tardar. Si no aparece, envía una captura del error y de la barra de direcciones.

No abras `index.html` con doble clic si no funciona: algunos módulos de JavaScript y funciones XR requieren un servidor.

## Para probar el Quest 3S más adelante
WebXR normalmente requiere HTTPS cuando el visor abre la página desde otro dispositivo. Tendremos que publicar la aplicación en un alojamiento HTTPS o montar un servidor HTTPS local, y después abrir esa dirección en el navegador del Quest. No hace falta hacerlo todavía.

## Créditos y licencias
- Modelo: Écorché, https://github.com/Charleeh/ecorche — CC BY-SA 4.0.
- Basado en BodyParts3D y Z-Anatomy; revisa los créditos y licencias completos en el repositorio fuente antes de redistribuir el proyecto.
- Código de la aplicación escrito para este proyecto educativo.
- Three.js: https://threejs.org/ — licencia MIT.

Atribución sugerida:
“Écorché (https://github.com/Charleeh/ecorche), CC BY-SA 4.0. Basado en BodyParts3D, © The Database Center for Life Science, CC BY 4.0, y Z-Anatomy por Gauthier Kervyn, CC BY-SA 4.0.”

El modelo y la información son para educación, no para uso clínico. Este prototipo no es todavía un atlas completo: incluye esqueleto y músculos, no órganos, nervios, vasos sanguíneos ni fichas anatómicas exhaustivas.
