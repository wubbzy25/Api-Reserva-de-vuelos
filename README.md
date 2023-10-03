# Descripcion General

Este proyecto tiene como objetivo desarrollar un sistema de reservas de vuelos en línea que permita a los usuarios buscar, seleccionar y reservar vuelos disponibles. El sistema consta de varios microservicios que trabajan juntos para proporcionar esta funcionalidad

**Backend del Sistema de Reservas de Vuelos:**

1. **Microservicio de Autenticación:**

 * Gestiona la autenticación y autorización de usuarios.
 * Proporciona endpoints para registro, inicio de sesión y gestión de perfiles de usuario.
 * Genera y verifica tokens JWT para la autenticación y autorización.
 * Almacena información de usuarios en una base de datos segura.

2. **Microservicio de Búsqueda de Vuelos:**
 * Proporciona una API para buscar vuelos disponibles.
 * Se integra con servicios de terceros o bases de datos para obtener información sobre vuelos, aerolíneas, horarios y precios.
 * Ofrece filtrado avanzado de búsqueda, como origen, destino, fecha de salida, fecha de regreso, escalas, etc.
 * Devuelve resultados de búsqueda en formato JSON.

3. **Microservicio de Reservas:**
 * Gestiona la reserva de vuelos y su procesamiento.
 * Verifica la disponibilidad de asientos en vuelos seleccionados.
 * Realiza el proceso de pago utilizando una pasarela de pago segura.
 * Almacena información de reservas en una base de datos.

4. **Microservicio de Notificaciones:**
 * Envía notificaciones por correo electrónico o mensajes SMS para confirmaciones de reservas, actualizaciones de vuelos, etc.
 * Utiliza un servicio de envío de correo electrónico o mensajes SMS para entregar notificaciones a los usuarios.
