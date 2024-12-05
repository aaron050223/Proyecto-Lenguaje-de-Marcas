# Documentación del Proyecto Web

## Proyecto de Aarón Gallardo Canto

## Fase 1: Planificación del Proyecto (Wireframe y Estructura HTML)

### Análisis de requisitos y objetivos del proyecto
El objetivo de este proyecto era crear una página web dedicada a la venta de material deportivo, algo parecido a lo que hacen Decathlon o Sprinter. La idea era hacer una web sencilla, intuitiva y cómoda de usar para cualquier tipo de público, sin importar su edad o experiencia navegando en internet. En cuanto a los colores, opté por tonos que no cansen la vista y que hagan un buen contraste. Esto no solo ayuda a que todo se vea más limpio, sino que también hace que las partes importantes, como los botones o las secciones destacadas, llamen la atención sin ser molestas.

---

### Creación de un wireframe

Primero voy a hablar de algo que está en todas las ventanas, como lo son el header y el footer. El header al final termina estando arriba del todo, sin ningún espacio, mientras que en el footer termino añadiendo políticas de privacidad, de empresa y cookies, y quitando las redes sociales.

Una de las ventanas la cual carece de wireframe son estas últimas, las de políticas y cookies. Las cuales pasé por alto a la hora de hacer los wireframe. Al igual que la de perfil, la cual he ido haciendo sobre la marcha.

**_Foto de inicio_**

![wireframe](imagen/readme/Inicio%20.png)

La pestaña de inicio considero que es bastante parecida. La ventana deslizante del wireframe termina siendo una ventana donde se promocionan unas botas. También se diferencia el “PRODUCTOS DESTACADOS”, el cual termina siendo “NOVEDADES” y se sitúa más en el centro.

**_Inicio con el menú abierto_**

![wireframe](imagen/readme/Inicio%20con%20menu%20abierto.png)

Se podría decir que es similar pero a la vez muy distinto. El menú de hamburguesa termina estando a la derecha y con únicamente 3 opciones.

**_Cesta_**

![wireframe](imagen/readme/Modelos%20de%20un%20producto%20copy.png)

La cesta sí que ha sufrido bastantes cambios. En la web opté por introducir todo el contenido dentro de una caja, ya que lo vi mejor presentado.

**_Menús_**

![wireframe](imagen/readme/Modelos%20de%20un%20producto.png)

Esta pestaña considero que es bastante similar. En el wireframe fui bastante ambicioso y puse una gran cantidad de productos. Luego en la web opté por incluir menos y para que no quedara mal puse únicamente 2 productos por fila.

**_Especificaciones_**

![wireframe](imagen/readme/Espicificaciones%20del%20producto.png)

Esta pestaña creo que es la que más se parece. Es muy muy parecida, con la única diferencia de que eliminé el botón “comprar”. Esto debido a que lo vi mejor sin este y pienso que quedaba mejor en la cesta. Además de la inclusión de “PRODUCTOS SIMILARES” en la parte inferior.

---

### Estructura HTML planificada
En el header tengo localizado el logo de la web (el cual sirve para que nos lleve a la página de inicio), en la parte central tengo un placeholder para buscar productos de la tienda. En la parte superior derecha nos encontramos un botón de “3 puntos” que si le damos nos mostrará un menú de hamburguesa con varios tipos de productos que tenemos en la tienda.

También nos encontramos en esa zona una cesta donde podemos ver qué productos hemos seleccionado y donde podemos pagar. Por último, nos encontramos con el perfil, donde podemos meter nuestro correo y contraseña para poder tener una cuenta, pedir artículos y estar informados de novedades que se producen en nuestra tienda.

El main varía mucho dependiendo de la ventana, pero es donde se encuentra el cuerpo de la pestaña en general.

En el footer se añaden las políticas de la tienda, estando estas en mi opinión bastante claras.

---

## Fase 2: Diseño y Desarrollo del Frontend (HTML y CSS)

### Configuración del entorno de desarrollo
Para ello, creé una serie de carpetas:
- `/css`: Donde se guardaba lo que venía siendo la estética de la web.
- `/imagen`: Donde dentro de cada una tiene divididas en header/main/footer las imágenes que iba a usar más tarde en la web. De esta forma las tenía divididas dependiendo en qué parte de la web iban a estar.
- Por último, los “.html” no los tenía en ninguna carpeta, ya que así lo consideraba más cómodo y más sencillo de utilizar.

---

### Desarrollo de la estructura HTML
Este paso implica construir la base de tu página web utilizando HTML, siguiendo el plan definido en la fase de planificación (como el wireframe o el esquema). Aquí están los aspectos clave:

#### a) Uso de etiquetas semánticas:
- Las etiquetas semánticas ayudan a que el navegador y las herramientas de accesibilidad comprendan mejor el contenido. Ejemplos:
    - `<header>`: Encabezado de la página, suele contener el logo, la barra de búsqueda y la navegación.
    - `<main>`: Área principal de contenido.
    - `<footer>`: Contiene la información final como enlaces legales (políticas, términos) y el copyright.

#### b) Organización lógica del contenido:
- El contenido debe estar estructurado de manera clara y jerárquica. Por ejemplo:
    - Usa `<h1>` para el título principal de la página y `<h2>`, `<h3>` para subtítulos.
    - Divide el contenido en secciones lógicas, como una sección para productos, otra para contacto, etc.
    - Evita usar etiquetas genéricas como `<div>` o `<span>` si hay etiquetas semánticas disponibles.

---

### Aplicación de estilos CSS
Una vez que tienes la estructura HTML, se aplican los estilos visuales con CSS. Esto incluye el diseño visual, los colores, las fuentes, el espaciado y la adaptabilidad a diferentes dispositivos.

#### a) Vincular la hoja de estilos:
Usa `<link>` en el `<head>` de tu HTML para conectar el CSS:
```html
<link rel="stylesheet" href="css/style.css">
```
#### b) Definir la presentación visual:
- Establece un diseño atractivo y consistente:
  - Colores, fuentes, tamaños y espaciados.
  - Alineación de elementos (usa `flexbox` o `grid` para diseños avanzados).

#### c) Hacer el diseño responsive:
- Utiliza media queries para adaptar la web a pantallas pequeñas (móviles) y grandes (PC):
```css
body {
    font-family: Arial, sans-serif;
    background-color: #f0f0f0;
}

/* Estilos para pantallas pequeñas */
@media (max-width: 768px) {
    body {
        background-color: #ffffff;
    }
    header {
        flex-direction: column;
    }
}
```
# Fase 3: Implementación y Validación del Código

La verdad es que al validar el codigo me dio bastante problemas, por lo que validarlo me ayudo bastante a localizar mis fallos y poder limpiarlo un poco
