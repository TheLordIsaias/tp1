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

-.env
- config.json

**Ignorar rutas específicas**

- /src/config.json