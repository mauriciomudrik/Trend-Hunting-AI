# Eliminación de Usuario

## 🇪🇸 Español: ¿Qué sucede al eliminar un usuario?

Al solicitar la eliminación de un usuario a través del panel de administración, tiene a su disposición las siguientes opciones para gestionar los datos vinculados a esa cuenta:

1. **Crear copia de seguridad y enviar al correo electrónico del usuario**:
   - El sistema recopilará todos los datos del usuario, así como los datos de los proyectos en los que sea el único propietario, incluyendo publicaciones recopiladas, métricas y claves.
   - Un archivo JSON estructurado que contenga esta información será enviado automáticamente como archivo adjunto a la dirección de correo electrónico registrada del usuario.

2. **Eliminar todos los datos relacionados (proyectos, publicaciones, configuraciones de API y OAuth)** (Deep Wipe):
   - Si esta opción está activada, no solo se eliminará el usuario. El sistema borrará permanentemente todos los proyectos en los que este usuario sea el miembro exclusivo.
   - Esto garantiza la terminación inmediata de las recopilaciones (publicaciones), claves de API (Configuraciones API) y sesiones activas de OAuth o scraping registradas bajo la cuenta del usuario para esos proyectos.
   - **Auditoría de Eliminación (Registro)**: Siempre que se ejecute esta acción profunda, la API del sistema creará internamente un archivo de texto con el registro detallado. Este registro enumerará cada proyecto eliminado y describirá cada clave API o OAuth eliminada, permitiendo el cumplimiento normativo y ratificando la eliminación de activos digitales confidenciales.
