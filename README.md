Curso «Aspectos básicos de Android con Compose».

La carpeta «Introduction» contiene el código de los ejercicios «Crea y usa variables en Kotlin» y «Cómo crear y usar funciones en Kotlin» de la sección «Introducción a la programación en Kotlin».
La carpeta «GreetingCard» contiene el código de los ejercicios «Create your first Android app» y «Run your first app on the Android Emulator» de la sección «Configuración de Android Studio».
La carpeta «HappyBirthday» contiene el código de los ejercicios «Compila una app simple con elementos de texto que admiten composición» y «Cómo agregar imágenes a tu app para Android» de la sección «Crea un diseño básico».

Introduction:
Estos ejercicios ayudan a una comprensión básica del uso de variables y funciones en el entorno Kotlin.

GreetingCard:
La clase MainActivity hereda de ComponentActivity y, dentro del método onCreate, configura el diseño visual de la aplicación. La función setContent permite definir la interfaz de usuario usando una estructura de diseño declarativa.
El uso de Scaffold proporciona una base para implementar patrones de diseño comunes en la interfaz de usuario. Dentro de Scaffold, se llama a una función composable Greeting que recibe un nombre y un modificador como parámetros. Greeting muestra un mensaje en un Surface con fondo de color cian, que contiene un Text con el mensaje "Hi, my name is [nombre]".
Finalmente, la función GreetingPreview utiliza la anotación @Preview para mostrar una vista previa en el entorno de desarrollo, permitiendo ver cómo se verá la interfaz con el nombre "Nicolò".

HappyBirthday:
En MainActivity, el método onCreate configura el diseño visual con setContent, aplicando el tema HappyBirthdayTheme y usando Surface para definir el contenedor principal.
Dentro de Surface, se llama a GreetingImage, una función composable que recibe un mensaje y un remitente como parámetros. GreetingImage muestra una imagen de fondo (androidparty) con transparencia, y encima coloca el texto de felicitación, usando la función GreetingText. Esta última organiza el texto en una columna centrada, ajustando el tamaño de fuente para crear un impacto visual: el mensaje principal tiene una fuente grande (100.sp) y el remitente se muestra con una fuente más pequeña.
Finalmente, BirthdayCardPreview proporciona una vista previa de la tarjeta en el entorno de desarrollo, permitiendo ver cómo quedará el diseño completo con el mensaje y la imagen.