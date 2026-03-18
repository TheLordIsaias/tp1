# tp1
## **¿Por qué es conveniente incluirlo?**

Incluir .gitignore es importante porque:

**1. Seguridad**

Evita subir información sensible:

- Contraseñas
- Claves API
- Configuraciones privadas

**2. Mantiene limpio el repositorio**

No se suben archivos innecesarios como:

- Archivos temporales
- Cachés
-Archivos del sistema

**3. Mejora el rendimiento**

Menos archivos equivale a un repositorio más liviano y rápido.

**4. Facilita el trabajo en equipo**

Cada desarrollador puede tener configuraciones locales sin afectar a otros.

## ¿Cuándo se debe hacer?

Lo ideal es crear el .gitignore desde el inicio del proyecto, antes del primer commit.

**¿Por qué?** Porque así evitas que archivos innecesarios entren al historial de Git.

¿Cómo configurar .gitignore?

Se configura escribiendo reglas simples dentro del archivo.

## Reglas básicas

**Ignorar por extensión**

- *.log
- *.tmp
**Ignorar carpetas**

- node_modules/
- dist/
- build/

**Ignorar archivos específicos**

- .env
- config.json

**Ignorar rutas específicas**

- /src/config.json

## Punto 3

# Codigo Misterioso:

El codigo misterioso, invierte un numero, lo divide por dos y finalmente suma los digitos del numero invertido a si mismo. El cambio de los nombres de las variables estan hechos para respestar la convencion de nombres "camelCase" siendo lo mas directo posible con respecto a lo que hacen las funciones o que almacenan las variables.

# Codigo sin Funcionar:

El primer error es logico que se observa en la funcion, ya que al ser void y usar pasaje por valor, ese calculo (El de duplicar el numero) se pierde al terminar la funcion. Para ello simplemente se pasa por referencia la variable.

El segundo error notorio tiene que ver con como se hace el scanf, ya que la variable valor1 no se estaba pasando como el espacio de memoria.

Existe un tercer error y tiene que ver con una modificacion necesaria para el primer error, que es que la misma espera recibir un puntero, el cual ademas es necesario para poder tener un resultado despues. Por lo tanto se necesito crear una variable puntero al valor1 para poder pasarla.

Hubo un ultimo error de sintaxis y es que al final faltaba un ";" luego del return 0