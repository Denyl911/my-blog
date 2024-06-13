<script setup>
const route = useRoute();
const posts = ref([
  {
    id: 1,
    title: 'La Revolución Tecnológica de las Inteligencias Artificiales',
    desc: `<p class="mb-4">En la última década, hemos sido testigos de una verdadera revolución tecnológica protagonizada por las inteligencias artificiales (IA). Estos sistemas inteligentes han transformado profundamente múltiples industrias y aspectos de nuestra vida cotidiana. En este post, exploraremos cómo las IA están cambiando el mundo y cuáles son las implicaciones de esta revolución tecnológica.</p>
        
        <h2 class="text-2xl font-semibold mt-6 mb-2">1. Aplicaciones en Diversos Sectores</h2>
        <p class="mb-4">Las IA están presentes en una amplia gama de sectores, desde la atención médica hasta la industria automotriz. En medicina, por ejemplo, se utilizan para diagnósticos más precisos y personalizados. En el campo financiero, las IA analizan datos financieros en tiempo real para tomar decisiones de inversión. En el transporte, están detrás de los avances en vehículos autónomos.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">2. Aprendizaje Automático y Redes Neuronales</h2>
        <p class="mb-4">El aprendizaje automático (Machine Learning) es el corazón de muchas aplicaciones de IA. Las redes neuronales, inspiradas en el funcionamiento del cerebro humano, son utilizadas para reconocimiento de imágenes, procesamiento del lenguaje natural y otras tareas complejas. Estos sistemas aprenden de datos y experiencias pasadas para mejorar su rendimiento con el tiempo.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">3. Ética y Responsabilidad</h2>
        <p class="mb-4">La revolución de las IA también plantea desafíos éticos y de responsabilidad. El uso de datos masivos y la toma de decisiones automatizada pueden generar preocupaciones sobre la privacidad, el sesgo algorítmico y la transparencia en las decisiones tomadas por las máquinas. Es fundamental abordar estos temas para garantizar un desarrollo tecnológico ético y responsable.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">4. Impacto en el Empleo y la Sociedad</h2>
        <p class="mb-4">La automatización impulsada por las IA está transformando el mercado laboral. Si bien crea nuevas oportunidades en áreas como la programación de IA y la gestión de datos, también plantea preocupaciones sobre la pérdida de empleos en sectores automatizables. La sociedad debe adaptarse a estos cambios y promover políticas que fomenten una transición justa y equitativa.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">5. Avances Futuros y Desafíos</h2>
        <p class="mb-4">El futuro de las IA promete avances aún más emocionantes, como la inteligencia artificial general (AGI) que podría igualar o superar la inteligencia humana en todas las áreas. Sin embargo, esto también plantea desafíos técnicos y éticos significativos, como la seguridad de los sistemas AGI y su impacto en la sociedad.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">Conclusión</h2>
        <p class="mb-4">La revolución tecnológica de las inteligencias artificiales está en pleno apogeo y seguirá transformando nuestro mundo de formas que apenas podemos imaginar. Es crucial abordar los desafíos éticos, sociales y técnicos que surgen de esta revolución para asegurar que las IA se desarrollen de manera responsable y beneficien a la humanidad en su conjunto.</p>`,
    date: '13 junio 2024',
    img: '/img/ai.jpg'
  },
  {
    id: 2,
    title: 'Comandos Esenciales de Linux que Debes Conocer',
    desc: `<p class="mb-4">Linux es un sistema operativo poderoso y flexible que se utiliza ampliamente en servidores y computadoras personales. Conocer los comandos básicos de Linux te permite gestionar archivos, administrar procesos y configurar tu sistema de manera eficiente. En este post, exploraremos algunos de los comandos esenciales que todos deberían conocer en Linux.</p>
        
        <h2 class="text-2xl font-semibold mt-6 mb-2">1. ls - Listar Archivos y Directorios</h2>
        <p class="mb-4">El comando <code>ls</code> se utiliza para listar archivos y directorios en el directorio actual. Algunas opciones comunes incluyen:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>ls</code>: lista los archivos y directorios en el directorio actual.</li>
            <li><code>ls -l</code>: muestra la lista en formato largo, incluyendo permisos, propietario, grupo, tamaño y fecha de modificación.</li>
            <li><code>ls -a</code>: muestra todos los archivos, incluyendo los ocultos (que comienzan con un punto).</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">2. cd - Cambiar de Directorio</h2>
        <p class="mb-4">El comando <code>cd</code> se utiliza para cambiar de directorio. Algunos ejemplos son:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>cd directorio</code>: cambia al directorio especificado.</li>
            <li><code>cd ..</code>: sube un nivel en la jerarquía de directorios.</li>
            <li><code>cd ~</code>: cambia al directorio de inicio del usuario.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">3. mkdir - Crear Directorios</h2>
        <p class="mb-4">El comando <code>mkdir</code> se utiliza para crear directorios. Por ejemplo:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>mkdir carpeta</code>: crea un directorio llamado "carpeta".</li>
            <li><code>mkdir -p carpeta/subdirectorio</code>: crea la carpeta "carpeta" y dentro de ella el subdirectorio "subdirectorio".</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">4. rm - Eliminar Archivos y Directorios</h2>
        <p class="mb-4">El comando <code>rm</code> se utiliza para eliminar archivos y directorios. Ten cuidado al usar este comando, ya que los archivos eliminados no se pueden recuperar fácilmente. Algunos ejemplos son:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>rm archivo</code>: elimina el archivo especificado.</li>
            <li><code>rm -r directorio</code>: elimina el directorio y su contenido de forma recursiva.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">5. cp - Copiar Archivos y Directorios</h2>
        <p class="mb-4">El comando <code>cp</code> se utiliza para copiar archivos y directorios. Por ejemplo:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>cp archivo destino</code>: copia el archivo en el destino especificado.</li>
            <li><code>cp -r directorio destino</code>: copia el directorio y su contenido en el destino de forma recursiva.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">6. mv - Mover y Renombrar Archivos y Directorios</h2>
        <p class="mb-4">El comando <code>mv</code> se utiliza para mover y renombrar archivos y directorios. Por ejemplo:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>mv archivo destino</code>: mueve el archivo al destino especificado.</li>
            <li><code>mv archivo nuevo_nombre</code>: renombra el archivo con el nuevo nombre.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">7. nano - Editor de Texto en Terminal</h2>
        <p class="mb-4">El comando <code>nano</code> se utiliza para abrir un editor de texto en la terminal. Por ejemplo:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>nano archivo</code>: abre el archivo especificado en el editor nano.</li>
            <li>Usa las teclas de navegación (flechas) y las combinaciones de teclas (Ctrl + O para guardar, Ctrl + X para salir) para editar y guardar el archivo.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">8. grep - Buscar Patrones en Archivos</h2>
        <p class="mb-4">El comando <code>grep</code> se utiliza para buscar patrones de texto en archivos. Por ejemplo:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>grep palabra archivo</code>: busca la palabra especificada en el archivo.</li>
            <li><code>grep -r palabra directorio</code>: busca la palabra en todos los archivos dentro del directorio de forma recursiva.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">9. ps - Mostrar Procesos</h2>
        <p class="mb-4">El comando <code>ps</code> se utiliza para mostrar los procesos en ejecución. Algunas opciones comunes incluyen:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>ps</code>: muestra los procesos del usuario actual.</li>
            <li><code>ps aux</code>: muestra todos los procesos del sistema en formato detallado.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">10. chmod - Cambiar Permisos de Archivos</h2>
        <p class="mb-4">El comando <code>chmod</code> se utiliza para cambiar los permisos de archivos y directorios. Por ejemplo:</p>
        <ul class="list-disc list-inside mb-4">
            <li><code>chmod +x archivo</code>: otorga permiso de ejecución al archivo.</li>
            <li><code>chmod u+r archivo</code>: otorga permiso de lectura al propietario del archivo.</li>
        </ul>
        <h2 class="text-2xl font-semibold mt-6 mb-2">Conclusión</h2>
        <p class="mb-4">Estos son solo algunos de los comandos esenciales que todos deberían conocer en Linux. Dominar estos comandos te ayudará a gestionar tu sistema de manera eficiente y a realizar tareas básicas de administración de archivos y procesos. ¡Explora y experimenta con estos comandos para mejorar tu experiencia en Linux!</p>
        <p class="mt-6">Espero que esta guía de comandos esenciales de Linux te haya sido útil. Si tienes alguna pregunta o deseas más información sobre algún comando en particular, ¡no dudes en preguntar!</p>`,
    date: '12 junio 2024',
    img: '/img/term.jpg'
  },
  {
    id: 3,
    title: 'Explorando los Frameworks de Desarrollo Web',
    desc: `<p class="mb-4">Los frameworks de desarrollo web han revolucionado la forma en que se construyen y mantienen aplicaciones web. Estas herramientas ofrecen un conjunto de bibliotecas, estructuras y patrones de diseño que agilizan el proceso de desarrollo y mejoran la eficiencia de los equipos de desarrollo. En este post, vamos a explorar algunos de los frameworks más populares en el mundo del desarrollo web.</p>
        
        <h2 class="text-2xl font-semibold mt-6 mb-2">1. ReactJS</h2>
        <p class="mb-4">**Características Principales:**</p>
        <ul class="list-disc list-inside mb-4">
            <li>Desarrollado por Facebook, ReactJS es un framework de código abierto para construir interfaces de usuario interactivas.</li>
            <li>Utiliza un enfoque basado en componentes que facilita la creación y reutilización de componentes UI.</li>
            <li>Su uso de JSX (una sintaxis que combina HTML y JavaScript) permite escribir código más legible y mantenible.</li>
            <li>ReactJS es altamente escalable y es utilizado por empresas como Facebook, Instagram y Airbnb.</li>
        </ul>
        <h2 class="text-2xl font-semibold mt-6 mb-2">2. Angular</h2>
        <p class="mb-4">**Características Principales:**</p>
        <ul class="list-disc list-inside mb-4">
            <li>Desarrollado por Google, Angular es un framework completo que abarca todo el ciclo de vida de una aplicación web.</li>
            <li>Utiliza el patrón MVC (Model-View-Controller) para separar la lógica de presentación de la lógica de negocio.</li>
            <li>Proporciona herramientas para la creación de componentes, enrutamiento, manejo de formularios y comunicación con servidores.</li>
            <li>Angular es ampliamente utilizado en aplicaciones empresariales y de gran escala.</li>
        </ul>
        <h2 class="text-2xl font-semibold mt-6 mb-2">3. Vue.js</h2>
        <p class="mb-4">**Características Principales:**</p>
        <ul class="list-disc list-inside mb-4">
            <li>Vue.js es un framework progresivo de código abierto para construir interfaces de usuario.</li>
            <li>Se enfoca en la capa de vista de una aplicación y es fácilmente integrable con otros frameworks y bibliotecas.</li>
            <li>Tiene una curva de aprendizaje suave y es conocido por su simplicidad y flexibilidad.</li>
            <li>Vue.js es utilizado por empresas como Alibaba, Xiaomi y Adobe.</li>
        </ul>
        <h2 class="text-2xl font-semibold mt-6 mb-2">4. Express.js</h2>
        <p class="mb-4">**Características Principales:**</p>
        <ul class="list-disc list-inside mb-4">
            <li>Express.js es un framework de desarrollo web para Node.js, que permite construir aplicaciones web y APIs de manera rápida y eficiente.</li>
            <li>Proporciona una capa de abstracción sobre el servidor HTTP de Node.js, simplificando el manejo de rutas, middleware y otras funcionalidades.</li>
            <li>Es ligero y flexible, lo que lo hace ideal para aplicaciones de cualquier tamaño.</li>
            <li>Express.js es ampliamente utilizado en el desarrollo de aplicaciones web basadas en Node.js.</li>
        </ul>
        <h2 class="text-2xl font-semibold mt-6 mb-2">5. Django</h2>
        <p class="mb-4">**Características Principales:**</p>
        <ul class="list-disc list-inside mb-4">
            <li>Django es un framework de desarrollo web de alto nivel escrito en Python.</li>
            <li>Ofrece un conjunto completo de herramientas para construir aplicaciones web de manera rápida y segura.</li>
            <li>Incluye funcionalidades como el ORM (Object-Relational Mapping) para interactuar con la base de datos, un sistema de administración de contenido, autenticación de usuarios y más.</li>
            <li>Django es utilizado por empresas como Instagram, Pinterest y The Washington Times.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">Conclusión</h2>
        <p class="mb-4">Los frameworks de desarrollo web juegan un papel crucial en la creación de aplicaciones web modernas y eficientes. La elección del framework adecuado depende de los requisitos específicos del proyecto, el conocimiento del equipo de desarrollo y otros factores como la escalabilidad y la facilidad de mantenimiento.</p>
        <p class="mb-4">Al explorar y familiarizarse con estos frameworks, los desarrolladores pueden mejorar su productividad y construir aplicaciones web de alta calidad que satisfagan las necesidades de los usuarios y las empresas.</p>

        <p class="mt-6">Espero que esta exploración de los frameworks de desarrollo web te haya sido útil. Si tienes alguna pregunta o deseas más información sobre algún framework en particular, ¡no dudes en preguntar!</p>`,
    date: '10 junio 2024',
    img: '/img/web2.jpg'
  },
  {
    id: 4,
    title: 'Diferencias entre SOAP y REST',
    desc: `<p class="mb-4">En el mundo de los servicios web, SOAP (Simple Object Access Protocol) y REST (Representational State Transfer) son dos de los protocolos más utilizados. Ambos tienen sus propias características, ventajas y desventajas. En este post, exploraremos las principales diferencias entre SOAP y REST para ayudarte a comprender cuál puede ser la mejor opción para tu proyecto.</p>
        
        <h2 class="text-2xl font-semibold mt-6 mb-2">1. Definición y Enfoque</h2>
        <h3 class="text-xl font-semibold mt-4 mb-2">SOAP:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>SOAP es un protocolo basado en XML que fue diseñado para permitir la comunicación entre aplicaciones a través de Internet.</li>
            <li>Sigue un estándar riguroso y utiliza un conjunto de reglas para estructurar los mensajes, lo que garantiza una comunicación más segura y confiable.</li>
            <li>SOAP es independiente del lenguaje y del sistema operativo.</li>
        </ul>
        <h3 class="text-xl font-semibold mt-4 mb-2">REST:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>REST es un estilo de arquitectura que utiliza el protocolo HTTP para la comunicación.</li>
            <li>No es un protocolo en sí, sino una forma de diseñar servicios web que aprovecha las características y funcionalidades del HTTP.</li>
            <li>RESTful APIs son generalmente más sencillas y ligeras en comparación con SOAP.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">2. Formato de Mensajes</h2>
        <h3 class="text-xl font-semibold mt-4 mb-2">SOAP:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>Utiliza XML para estructurar los mensajes.</li>
            <li>Los mensajes SOAP son más pesados debido al uso extensivo de XML.</li>
            <li>SOAP requiere una cabecera específica y un cuerpo en el mensaje, lo que añade más sobrecarga.</li>
        </ul>
        <h3 class="text-xl font-semibold mt-4 mb-2">REST:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>Puede usar múltiples formatos de datos como XML, JSON, YAML y texto plano, siendo JSON el más popular debido a su ligereza y facilidad de uso.</li>
            <li>Los mensajes REST son generalmente más ligeros y más fáciles de manejar en comparación con SOAP.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">3. Transporte y Protocolos</h2>
        <h3 class="text-xl font-semibold mt-4 mb-2">SOAP:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>SOAP puede utilizar varios protocolos de transporte como HTTP, SMTP, TCP, entre otros.</li>
            <li>Debido a su flexibilidad con los protocolos de transporte, SOAP es adecuado para aplicaciones que requieren una alta fiabilidad y seguridad.</li>
        </ul>
        <h3 class="text-xl font-semibold mt-4 mb-2">REST:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>REST se basa principalmente en el protocolo HTTP.</li>
            <li>Hace uso de los métodos HTTP estándar como GET, POST, PUT, DELETE para realizar operaciones CRUD (Crear, Leer, Actualizar, Borrar).</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">4. Estándares y Seguridad</h2>
        <h3 class="text-xl font-semibold mt-4 mb-2">SOAP:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>SOAP tiene estándares bien definidos para la seguridad (WS-Security) y transacciones (WS-AtomicTransaction).</li>
            <li>Proporciona una mayor seguridad debido a la implementación de estos estándares, lo que es crucial para aplicaciones empresariales.</li>
        </ul>
        <h3 class="text-xl font-semibold mt-4 mb-2">REST:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>REST no tiene estándares específicos de seguridad integrados, pero puede utilizarse con mecanismos de seguridad HTTP como SSL/TLS.</li>
            <li>Es más adecuado para aplicaciones que no requieren un nivel alto de seguridad y transacciones complejas.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">5. Performance y Escalabilidad</h2>
        <h3 class="text-xl font-semibold mt-4 mb-2">SOAP:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>SOAP es más pesado y puede ser más lento debido a su formato XML y las reglas estrictas de procesamiento.</li>
            <li>La sobrecarga adicional puede afectar la performance en aplicaciones con alto tráfico.</li>
        </ul>
        <h3 class="text-xl font-semibold mt-4 mb-2">REST:</h3>
        <ul class="list-disc list-inside mb-4">
            <li>REST es generalmente más rápido y más eficiente debido a su menor sobrecarga y uso de JSON.</li>
            <li>Es más escalable y adecuado para aplicaciones web modernas que requieren una respuesta rápida y eficiente.</li>
        </ul>

        <h2 class="text-2xl font-semibold mt-6 mb-2">Conclusión</h2>
        <p class="mb-4">La elección entre SOAP y REST depende de los requisitos específicos de tu proyecto.</p>
        <ul class="list-disc list-inside mb-4">
            <li><strong>SOAP</strong> es ideal para aplicaciones que requieren alta seguridad, transacciones complejas y una comunicación confiable entre sistemas diferentes.</li>
            <li><strong>REST</strong> es más adecuado para aplicaciones web modernas que requieren una comunicación rápida, eficiente y flexible con diferentes formatos de datos.</li>
        </ul>
        <p class="mb-4">Ambos tienen sus propias ventajas y desventajas, y comprender estas diferencias te ayudará a tomar una decisión informada sobre cuál utilizar para tu proyecto.</p>

        <p class="mt-6">Espero que esta comparativa te haya sido útil. Si tienes alguna pregunta o necesitas más información, no dudes en dejar un comentario. ¡Feliz desarrollo!</p>`,
    date: '9 junio 2024',
    img: '/img/code.jpg'
  },
  {
    id: 5,
    title: 'Cómo Crear tu Propio Sitio Web Fácilmente',
    desc: `<p class="mb-4">¿Alguna vez has querido tener tu propio sitio web pero te has sentido abrumado por la complejidad del proceso? No te preocupes, crear un sitio web es más fácil de lo que piensas. Aquí te presento una guía paso a paso para que puedas tener tu propio sitio web en poco tiempo.</p>
        
        <h2 class="text-2xl font-semibold mt-6 mb-2">1. Planifica Tu Sitio Web</h2>
        <p class="mb-4">Antes de empezar, es importante tener claro el propósito de tu sitio web. ¿Será un blog, un portafolio, una tienda en línea o una página informativa? Define tu audiencia y los objetivos que quieres alcanzar con tu sitio.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">2. Elige un Nombre de Dominio</h2>
        <p class="mb-4">El nombre de dominio es la dirección de tu sitio web (por ejemplo, www.tusitio.com). Elige un nombre que sea fácil de recordar y represente el contenido de tu sitio. Puedes registrar tu dominio a través de servicios como GoDaddy, Namecheap o Google Domains.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">3. Selecciona un Proveedor de Hosting</h2>
        <p class="mb-4">El hosting es donde se almacenará tu sitio web. Hay muchas opciones disponibles como Bluehost, HostGator, y SiteGround. Muchos proveedores de hosting ofrecen paquetes que incluyen el registro del dominio y herramientas para construir tu sitio web.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">4. Elige una Plataforma de Construcción de Sitios Web</h2>
        <p class="mb-4">Para facilitar el proceso, te recomiendo usar una plataforma de construcción de sitios web como WordPress, Wix o Squarespace. Estas plataformas ofrecen plantillas prediseñadas y herramientas fáciles de usar para que puedas personalizar tu sitio sin necesidad de conocimientos avanzados de programación.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">5. Diseña Tu Sitio Web</h2>
        <p class="mb-4">Elige una plantilla que se adapte a tus necesidades y personalízala a tu gusto. Asegúrate de que tu sitio sea fácil de navegar y que el diseño sea atractivo. Incluye las secciones básicas como una página de inicio, una página sobre ti o tu negocio, una página de contacto y cualquier otra sección relevante.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">6. Añade Contenido</h2>
        <p class="mb-4">El contenido es la parte más importante de tu sitio web. Asegúrate de que sea relevante, atractivo y de alta calidad. Incluye textos, imágenes, videos y cualquier otro tipo de contenido que sea útil para tus visitantes.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">7. Optimiza para Motores de Búsqueda (SEO)</h2>
        <p class="mb-4">Para que tu sitio web sea fácilmente encontrado en los motores de búsqueda como Google, es importante optimizarlo para SEO. Utiliza palabras clave relevantes, crea contenido de calidad, y asegúrate de que tu sitio cargue rápidamente.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">8. Lanza Tu Sitio Web</h2>
        <p class="mb-4">Una vez que hayas terminado de diseñar y añadir contenido, revisa tu sitio para asegurarte de que todo funcione correctamente. Luego, ¡lánzalo! Comparte tu sitio web con amigos, familiares y en redes sociales para empezar a atraer visitantes.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">9. Mantén Tu Sitio Web Actualizado</h2>
        <p class="mb-4">Un sitio web exitoso requiere mantenimiento continuo. Actualiza regularmente el contenido, revisa las analíticas para entender el comportamiento de tus visitantes, y realiza mejoras basadas en esos datos.</p>

        <h2 class="text-2xl font-semibold mt-6 mb-2">Conclusión</h2>
        <p class="mb-4">Crear tu propio sitio web no tiene por qué ser complicado. Con las herramientas y plataformas disponibles hoy en día, puedes tener tu sitio web funcionando en poco tiempo. Sigue estos pasos y estarás en camino de tener un sitio web profesional y funcional que te ayudará a alcanzar tus objetivos. ¡Buena suerte!</p>
        
        <p class="mt-6">Espero que este post te haya sido útil. Si tienes alguna pregunta o necesitas ayuda adicional, no dudes en dejar un comentario. ¡Feliz construcción de tu sitio web!</p>`,
    date: '5 junio 2024',
    img: '/img/web1.jpg'
  },
]);

const post = ref({ id: 0, title: '...', desc: '...', date: '13 junio 2024' });
post.value = posts.value.find((el) => el.id == route.params.id);
useSeoMeta({
  title: post.value.title + ' | Denyl',
})
</script>

<template>
  <div class="text-center container mx-auto">
    <h1 class="text-4xl font-bold py-5">{{ post.title }}</h1>
    <div class="flex items-center justify-center gap-3 pb-4 pt">
      <img src="/img/user2.png" alt="User image" />
      <div class="text-left">
        <h5 class="font-bold">Denilson De La Rosa</h5>
        <p>{{ post.date }}</p>
      </div>
    </div>
    <img class="mx-auto rounded mb-2 w-9/12" :src="post.img" alt="Banner image" />
    <p class="text-3xl font-bold mb-5">. . .</p>
    <div class="text-justify mb-20 mx-5">
        <p v-html="post.desc"></p>
    </div>
  </div>
</template>
