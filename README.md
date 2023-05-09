![Tutorial de como manipular cookies en Javascript imagen 1](https://raw.githubusercontent.com/sergiecode/cookies-tutorial/master/cookies-tutorial%20%281%29.jpg)

![Tutorial de como manipular cookies en Javascript imagen 2](https://raw.githubusercontent.com/sergiecode/cookies-tutorial/master/cookies-tutorial%20%282%29.jpg)

![Tutorial de como manipular cookies en Javascript imagen 3](https://raw.githubusercontent.com/sergiecode/cookies-tutorial/master/cookies-tutorial%20%283%29.jpg)

![Tutorial de como manipular cookies en Javascript imagen 4](https://raw.githubusercontent.com/sergiecode/cookies-tutorial/master/cookies-tutorial%20%284%29.jpg)

![Tutorial de como manipular cookies en Javascript imagen 5](https://raw.githubusercontent.com/sergiecode/cookies-tutorial/master/cookies-tutorial%20%285%29.jpg)

# Tutorial sobre cookies en JavaScript

Este tutorial describe cómo trabajar con cookies en JavaScript. Las cookies son pequeños archivos que se almacenan en el navegador del usuario y se utilizan para almacenar información relevante para el sitio web, como preferencias de usuario, información de inicio de sesión, etc.

## Crear una cookie

Para crear una cookie en JavaScript, puedes utilizar la propiedad `document.cookie`. El siguiente código crea una cookie con el nombre "username" y el valor "John":

    `document.cookie = "username=John";` 

## Leer una cookie

Para leer una cookie en JavaScript, puedes utilizar la propiedad `document.cookie` y la función `split()` para separar los pares clave-valor. El siguiente código muestra cómo leer la cookie "username":

    `const cookies = document.cookie.split("; ");
    for (let i = 0; i < cookies.length; i++) {
      const cookie = cookies[i].split("=");
      if (cookie[0] === "username") {
        console.log(cookie[1]);
      }
    }` 

## Modificar una cookie

Para modificar una cookie en JavaScript, simplemente crea una nueva cookie con el mismo nombre y un nuevo valor. El siguiente código modifica la cookie "username" con el nuevo valor "Jane":

    `document.cookie = "username=Jane";` 

## Eliminar una cookie

Para eliminar una cookie en JavaScript, simplemente establece su valor en vacío y su fecha de expiración en el pasado. El siguiente código elimina la cookie "username":

    `document.cookie = "username=; expires=Thu, 01 Jan 1970 00:00:00 UTC;";` 

¡Y eso es todo! Este tutorial cubre los fundamentos de cómo crear, leer, modificar y eliminar cookies en JavaScript. Si necesitas más información, asegúrate de consultar la documentación oficial de JavaScript sobre cookies.
