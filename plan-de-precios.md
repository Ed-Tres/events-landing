# edtres · Plan de precios (versión 1, acceso anticipado)

Fecha: 11 de noviembre de 2026
Estado: propuesta para validar con los primeros clientes. Los precios son de prueba.

## 1. Principio

El correo semanal va incluido en **todos** los planes. Es parte del valor del servicio para el planner, y el costo por evento es muy bajo. Los planes se diferencian por número de listas y de eventos, como ya está en la landing.

## 2. Planes

| Plan | Precio | Listas | Incluye |
|---|---|---|---|
| Evento sencillo | **$29** por evento | Hasta 1 | Página para invitados, reservas, lista de agradecimientos, resumen semanal por correo |
| Evento con varias listas | **$49** por evento | Hasta 3 | Todo lo anterior + exportación a hoja de cálculo |
| Evento grande | **$99** por evento | Hasta 10 | Todo lo anterior + soporte prioritario |
| Planner anual | **$249** al año | Hasta 10 por evento, hasta 10 eventos al año | Todo lo anterior, para planners con varios eventos |

Todos los precios se expresan en USD, y los impuestos aplicables se indicarán en la factura.

## 3. Qué incluye el correo semanal

**Estado actual:** próximamente. Hoy el resumen llega solo al administrador de edtres. El envío a cada planner requiere activar el plan Blaze, así que la landing lo presenta como próximamente hasta entonces.

- Un correo cada domingo, hasta la fecha del evento, con los regalos pendientes de cada evento publicado del planner.
- Enlace directo a la página de invitados y a cada lista de Amazon.
- Se deja de enviar automáticamente después de la fecha del evento.

No incluye recordatorios a los invitados: la plataforma no les pide correo, y el planner decide cómo comunicarse con ellos.

## 4. Costo estimado por evento (a verificar)

Supuestos: un evento con 30 regalos, 4 semanas de correos y un planner con 1 evento activo.

| Concepto | Estimado | Cómo se verifica |
|---|---|---|
| Función programada (una vez por semana) | Dentro de la cuota gratuita de Cloud Functions, según lo que conozco | Revisar la página de precios de Firebase/Google Cloud antes de activar Blaze |
| Lecturas de Firestore (regalos y eventos) | Centavos o menos por evento | Ver la sección de uso en la consola de Firebase |
| Correo transaccional (4 envíos por evento) | Dentro de la cuota gratuita de la mayoría de proveedores | Confirmar límites actuales del proveedor elegido |
| Alerta de presupuesto | Costo cero | Crear una alerta de $5 al mes en Google Cloud Billing |

Con estos supuestos, el costo variable por evento es mínimo frente al precio de $29. El riesgo real es el crecimiento: revisa el uso cada mes durante los primeros meses.

## 5. Acceso anticipado

- Los **primeros 10 clientes** reciben 30 % de descuento en su primer evento, a cambio de una llamada de 15 minutos y comentarios sinceros.
- El descuento no es acumulable y aplica solo al primer evento.

## 6. Condiciones que deben coincidir con los Términos de uso

- Pagos por evento, antes de activar la publicación.
- Cancelación antes de publicar la lista: reembolso completo dentro de 7 días del pago (así está en los términos).
- Sin renovación automática en los planes por evento.
- El plan anual se renueva solo si el cliente lo acepta explícitamente.

## 7. Dependencias antes de cobrar

1. **Medio de pago.** Verifica qué pasarela acepta cobros desde Panamá (por ejemplo PayPal o Stripe, según disponibilidad en tu cuenta) y si cobra en USD.
2. **Activación de cuentas de pago.** Hoy no hay cobros en la plataforma. Mientras tanto, activa los eventos de los clientes a mano, después de confirmar el pago.
3. **Plan Blaze.** Solo se activa cuando haya clientes que paguen por el correo individual. Hasta entonces, el resumen semanal llega solo a ti.
4. **Revisión legal.** Los precios y las condiciones deben coincidir con los Términos de uso y el aviso de privacidad, revisados por un abogado en Panamá.

## 8. Cambios pendientes en la landing

- Agregar "Resumen semanal por correo" a la lista de funciones y a cada plan.
- Mantener la oferta de los primeros 10 clientes.
- Revisar que la landing no prometa correos individuales a los planners hasta activar Blaze.

## 9. Indicadores a revisar cada mes

- Eventos vendidos por plan.
- Clientes que pasan del plan sencillo al de varias listas o al anual.
- Costo real de Firebase y del proveedor de correo, comparado con los ingresos.
- Número de descuentos de lanzamiento usados.
