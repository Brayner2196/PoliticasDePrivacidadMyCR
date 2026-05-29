# Política de Privacidad – Flutter Residential

**Última actualización:** 29 de mayo de 2026

---

## 1. Introducción

Flutter Residential ("la Aplicación") es una plataforma móvil multitenant para la gestión integral de conjuntos residenciales. Esta Política de Privacidad describe cómo recopilamos, usamos, almacenamos y protegemos la información personal de los usuarios.

Al usar la Aplicación, aceptas las prácticas descritas en este documento.

---

## 2. Responsable del Tratamiento

El responsable del tratamiento de datos es el **administrador del conjunto residencial** (Tenant Admin) que contrate el servicio. Flutter Residential actúa como encargado del tratamiento en nombre de dicho administrador.

Para consultas sobre privacidad, comunícate con el administrador de tu conjunto o escríbenos a: **soporte@flutterresidential.com**

---

## 3. Datos que Recopilamos

### 3.1 Datos de Registro y Autenticación
- Nombre completo
- Correo electrónico
- Contraseña (almacenada de forma encriptada, nunca en texto plano)
- Número de teléfono (opcional)
- Rol dentro del conjunto (Propietario, Inquilino, Administrador)

### 3.2 Datos de la Propiedad
- Número de unidad / apartamento
- Torre o bloque
- Información del conjunto residencial (nombre, dirección)

### 3.3 Datos de Pagos y Cobros
- Historial de pagos de administración y cuotas
- Métodos de pago utilizados (procesados por **Wompi** — no almacenamos datos de tarjetas)
- Referencias de transacción

### 3.4 Datos de Uso de la Aplicación
- Solicitudes (PQR) enviadas
- Reservas de áreas comunes
- Participación en votaciones
- Anuncios y comunicados leídos
- Interacciones con el Marketplace

### 3.5 Datos Técnicos
- Token de dispositivo para notificaciones push (Firebase Cloud Messaging)
- Versión del sistema operativo y del dispositivo
- Logs de errores y sesiones (para diagnóstico técnico)

---

## 4. Finalidad del Tratamiento

| Dato | Finalidad |
|------|-----------|
| Autenticación | Identificar y autenticar usuarios de forma segura |
| Datos de propiedad | Asociar al usuario a su unidad y conjunto |
| Pagos | Gestionar cobros, recibos y estados de cuenta |
| PQR | Tramitar peticiones, quejas y reclamos |
| Reservas | Administrar el uso de áreas comunes |
| Votaciones | Garantizar participación y registro de votos |
| Notificaciones | Enviar alertas relevantes sobre el conjunto |
| Datos técnicos | Mejorar el rendimiento y corregir errores |

---

## 5. Base Legal del Tratamiento

El tratamiento de datos personales se realiza bajo las siguientes bases legales:

- **Ejecución de contrato:** gestión de la relación entre residente y administración.
- **Obligación legal:** cumplimiento de normas aplicables a la propiedad horizontal.
- **Consentimiento:** para notificaciones push y comunicaciones opcionales.
- **Interés legítimo:** diagnóstico técnico y mejora del servicio.

---

## 6. Multi-Tenant y Aislamiento de Datos

La Aplicación opera en arquitectura **multitenant con aislamiento por esquema** (schema-per-tenant). Esto significa:

- Los datos de cada conjunto residencial están **completamente separados** de los demás.
- Ningún usuario puede acceder a datos de otro conjunto.
- El Tenant Admin solo gestiona los datos de su propio conjunto.

---

## 7. Pasarelas de Pago

Los pagos son procesados por **Wompi**. Flutter Residential **no almacena** números de tarjeta, CVV ni datos bancarios sensibles. Toda transacción financiera sigue los estándares **PCI DSS** de la pasarela correspondiente.

Para más información: [https://wompi.com/privacidad](https://wompi.com)

---

## 8. Servicios de Terceros

La Aplicación utiliza los siguientes servicios externos:

| Servicio | Finalidad | Política |
|----------|-----------|----------|
| **Firebase (Google)** | Autenticación, notificaciones push | [policies.google.com](https://policies.google.com/privacy) |
| **Wompi** | Procesamiento de pagos | [wompi.com](https://wompi.com) |
| **Servidor de API propio** | Backend Spring Boot con base de datos PostgreSQL | Ver sección 9 |

---

## 9. Almacenamiento y Seguridad

- Los datos se almacenan en servidores con **cifrado en reposo y en tránsito (HTTPS/TLS)**.
- Las credenciales se almacenan en el dispositivo usando **flutter_secure_storage** (iOS Keychain / Android Keystore).
- Los tokens de sesión tienen **expiración automática**.
- Acceso a datos restringido por **roles** (SUPER_ADMIN, TENANT_ADMIN, PROPIETARIO, INQUILINO).

---

## 10. Retención de Datos

| Tipo de dato | Período de retención |
|-------------|----------------------|
| Datos de cuenta activa | Mientras la cuenta esté activa |
| Historial de pagos | 5 años (obligación fiscal/legal) |
| PQR y solicitudes | 2 años |
| Logs técnicos | 90 días |
| Datos tras cierre de cuenta | 30 días para eliminación definitiva |

---

## 11. Derechos del Usuario

De acuerdo con la normativa aplicable (Ley 1581 de 2012 en Colombia), tienes derecho a:

- **Conocer** qué datos personales tuyos tenemos
- **Actualizar** o corregir tu información
- **Suprimir** tus datos (derecho al olvido)
- **Revocar** el consentimiento en cualquier momento
- **Presentar quejas** ante la Superintendencia de Industria y Comercio (SIC)

Para ejercer estos derechos, comunícate con el administrador de tu conjunto o a través de la sección **Configuración > Mi Cuenta** en la Aplicación.

---

## 12. Notificaciones Push

Las notificaciones push se envían mediante **Firebase Cloud Messaging (FCM)**. Puedes desactivarlas en cualquier momento desde:

- **Configuración de la App** → Notificaciones
- **Configuración del Sistema Operativo** → Aplicaciones → Flutter Residential

---

## 13. Menores de Edad

La Aplicación no está dirigida a personas menores de 18 años. Si detectamos que un menor ha proporcionado información personal sin consentimiento de sus padres o tutores, eliminaremos dicha información de inmediato.

---

## 14. Cambios a esta Política

Nos reservamos el derecho de actualizar esta Política de Privacidad. Cuando lo hagamos:

1. Actualizaremos la fecha al inicio del documento.
2. Notificaremos a los usuarios mediante la Aplicación o correo electrónico.
3. Los cambios significativos requerirán nueva aceptación explícita.

---

## 15. Contacto

Para preguntas, solicitudes o quejas relacionadas con privacidad:

- **Correo:** soporte@flutterresidential.com
- **Dentro de la app:** Configuración → Soporte → Privacidad

---

*Esta política está redactada conforme a la Ley 1581 de 2012 (Habeas Data), el Decreto 1377 de 2013 de Colombia, y los principios del GDPR como referencia de buenas prácticas internacionales.*
