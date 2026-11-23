# Decisiones de diseño

| ID | Decisión | Alternativa descartada | Motivo |
|---|---|---|---|
| D1 | Una sola clase Comprobante con atributo tipo | Clases Boleta y Factura | Casi los mismos datos |
| D2 | DetalleReserva entre Reserva y Habitacion | numeroHabitacion en Reserva | Una reserva puede incluir varias habitaciones |
| D3 | Estado del cuarto como atributo de Habitacion | Clase EstadoHabitacion con historial | Hoy no se registra el historial |
| D4 | Canal como atributo de Reserva | Clase Canal | Sin comportamiento propio |
| D5 | Lógica de negocio en clases gestoras | Reglas en el dominio | Dominio y pantallas simples |
| D6 | Reserva–Pago por agregación | Composición | El pago se conserva aunque se anule la reserva |
