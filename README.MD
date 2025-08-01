# Honeypot Básico con Docker y Docker Compose

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white) ![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)

Este proyecto despliega un honeypot web muy simple utilizando Docker y Nginx. El objetivo es simular una página de inicio de sesión vulnerable para registrar y analizar los intentos de acceso, sirviendo como una práctica fundamental para el uso de Docker en entornos de ciberseguridad.

---

### 🚀 Uso e Instalación

Para levantar el servicio, solo necesitas tener Docker y Docker Compose instalados.

1.  **Clona el repositorio:**

    ```bash
    git clone [https://github.com/TU_USUARIO/TU_REPOSITORIO.git](https://github.com/TU_USUARIO/TU_REPOSITORIO.git)
    cd TU_REPOSITORIO
    ```

2.  **Levanta el servicio:**

    ```bash
    docker-compose up -d
    ```

    El contenedor se construirá y se ejecutará en segundo plano.

3.  **Accede al Honeypot:**
    Abre tu navegador y ve a `http://localhost:8888`.

4.  **Monitoriza los logs:**
    Para ver los intentos de acceso en tiempo real, utiliza el siguiente comando:

    ```bash
    docker-compose logs -f
    ```

5.  **Detén el servicio:**
    Para detener y eliminar el contenedor y la red creada, ejecuta:
    ```bash
    docker-compose down
    ```

---

### 💡 Logros y Habilidades Demostradas

Este proyecto me ha permitido aplicar habilidades clave en Docker, demostrando mi capacidad para gestionar aplicaciones en contenedores de manera eficiente y profesional.

- **Simplifiqué el despliegue de la aplicación**, reduciendo los comandos de ejecución de 3 a 1, utilizando un archivo `docker-compose.yml` para definir el servicio de forma declarativa.

- **Creé una imagen de Docker optimizada**, asegurando un entorno de ejecución ligero y reproducible, mediante la escritura de un `Dockerfile` basado en `nginx:alpine`.

- **Implementé un sistema de monitorización de seguridad básico**, capaz de capturar en tiempo real todos los intentos de acceso al servicio, mediante el análisis de los logs del contenedor con el comando `docker-compose logs`.

- **Expuse el servicio web a la red local**, permitiendo el acceso desde cualquier dispositivo, a través de la configuración del mapeo de puertos en Docker Compose.

- **Garanticé la portabilidad del proyecto**, permitiendo que cualquier persona con Docker pueda replicar el entorno exacto con un solo comando, al empaquetar la aplicación y sus dependencias en una imagen de contenedor.
