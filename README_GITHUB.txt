PULSERA SOS — PWA V1.0
======================

CONTENIDO
- index.html: interfaz principal.
- styles.css: diseño adaptable a móvil y escritorio.
- app.js: configuración local, contactos, simulaciones e historial.
- manifest.webmanifest: instalación como PWA.
- service-worker.js: caché para uso sin conexión.
- assets/icon.svg: icono.

PUBLICAR EN GITHUB PAGES
1. Crea un repositorio NUEVO e independiente llamado: pulsera-sos-pwa
   No uses el repositorio APP-TKE ni el de mantenimiento PBB.
2. Sube el CONTENIDO de esta carpeta a la raíz de la rama main.
3. En GitHub: Settings > Pages.
4. En Build and deployment, elige Deploy from a branch.
5. Selecciona Branch: main y Folder: /(root). Guarda.
6. Espera a que GitHub Pages publique. La URL tendrá este formato:
   https://TU-USUARIO.github.io/pulsera-sos-pwa/

INSTALAR
- Android/Chrome: menú del navegador > Instalar aplicación o Añadir a pantalla de inicio.
- Ordenador: icono de instalación del navegador, si está disponible.
- iPhone/iPad: Safari > Compartir > Añadir a pantalla de inicio (cuando tengas uno).

CONFIGURACIÓN Y PRIVACIDAD
- Contactos y ajustes se guardan en localStorage del navegador.
- No se transmiten a GitHub ni a ningún servidor.
- Si borras los datos del sitio o cambias de navegador/dispositivo, se perderán.
- No introduzcas datos reales de contactos en un ordenador compartido.

ALCANCE Y SEGURIDAD
Esta V1 es una maqueta funcional de configuración y simulación.
NO incorpora Bluetooth BLE, detección real de caídas, GPS, backend, SMS,
llamadas, notificaciones push ni comunicación con servicios de emergencia.
No es un dispositivo médico ni un sistema de seguridad. No usar para emergencias.

PRÓXIMAS FASES
1. Definir el protocolo BLE definitivo de la placa XIAO nRF52840.
2. Implementar una capa de comunicación compatible con la plataforma elegida.
3. Crear backend de alertas con autenticación, ACK y deduplicación.
4. Integrar SMS/push únicamente en un entorno separado y tras pruebas.
5. Validar funcionamiento real, batería, pérdida de cobertura y fallos del sensor.
