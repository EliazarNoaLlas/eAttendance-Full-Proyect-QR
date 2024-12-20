# Sistema eAttendance Usando Código QR

¡Bienvenido al repositorio del Sistema eAttendance! Este sistema está diseñado para optimizar el proceso de asistencia usando códigos QR, asegurando un seguimiento de asistencia preciso y en tiempo real.

## Características

- **Generación de Códigos QR:** Los profesores pueden generar un código QR que representa una sesión. El código QR se muestra a los estudiantes para registrar la asistencia.

- **Tiempo de Expiración Personalizable:** Los profesores tienen la flexibilidad de establecer la duración durante la cual el código QR estará activo. Una vez que el tiempo establecido transcurre, el código QR se vuelve inválido.

- **Asistencia en Tiempo Real:** El sistema facilita el seguimiento de asistencia en tiempo real, permitiendo a los profesores registrar la asistencia de hasta 100 estudiantes en un minuto.

- **Integración con Aplicación Móvil:** Los estudiantes pueden usar la aplicación móvil dedicada desarrollada tanto para Android como para iOS usando Flutter. La aplicación permite escanear códigos QR de manera fluida para fines de asistencia.

- **Medidas Anti-Falsificación:** Para prevenir asistencias falsas, los estudiantes deben permanecer en la aplicación y conectados a la red después de escanear el código QR. Cualquier intento de cambiar de aplicación o modificar la red durante la sesión resultará en que la asistencia no sea registrada.

## Comenzando

### Prerrequisitos

- [Flutter](https://flutter.dev/) instalado para el desarrollo de la aplicación.
- [Java 17](https://openjdk.java.net/projects/jdk/17/) para el Backend de Asistencia.
- [STS (Spring Tool Suite)](https://spring.io/tools) recomendado como IDE para el desarrollo del backend.
- Base de datos MySQL con una base de datos llamada `attendance_system`. Configurar puerto y credenciales en `application.properties`.

### Instalación

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/smit-joshi814/eAttendance.git
   ```

2. **Backend (Java 17 & STS):**
    - Importar el proyecto backend en STS.
    - Configurar la base de datos en `application.properties`.
    - Ejecutar el proyecto como una Aplicación Spring Boot.

3. **Flutter (Frontend):**
    - Navegar al directorio `eattendance_student`.
    - Ejecutar `flutter pub get` para instalar dependencias.
    - Conectar un dispositivo o usar un emulador.
    - Ejecutar `flutter run` para lanzar la aplicación.

## Configuración

- **Configuración del Backend:**
    - La API del backend está construida usando Spring Boot.
    - Configurar la base de datos MySQL en `application.properties`.
    - Establecer el puerto apropiado para el backend.

- **Configuración del Frontend:**
    - La aplicación móvil está desarrollada usando Flutter.
    - Usar `flutter doctor` para asegurar que todas las dependencias estén instaladas.
    - Actualizar el SDK de Flutter si es necesario.
