# Registro de refactorización

| N.° | Problema encontrado | Cambio realizado | Resultado |
|---|---|---|---|
| R1 | GestorHostal manejaba reservas, cuartos y comprobantes (baja cohesión) | Se dividió en GestorReservas, GestorHabitaciones y GestorComprobantes | Cada clase tiene una sola responsabilidad |
| R2 | Reserva guardaba un solo número de habitación | Se creó DetalleReserva (composición) | Una reserva admite varias habitaciones |
| R3 | Reserva guardaba monto, método y fecha de pago | Se creó la clase Pago (agregación) | Se admiten pagos parciales y anulaciones |
| R4 | Recepcionista y Gerente repetían usuario y clave | Se creó la clase padre Usuario | Sin atributos duplicados |
| R5 | Las pantallas consultaban la base de datos directamente | Se creó el paquete Datos con repositorios | Cambiar la base de datos no afecta las pantallas |
| R6 | Varios atributos eran públicos | Pasaron a privados, con operaciones públicas | Mejor encapsulamiento |

## Indicadores

| Indicador | v0.1 | v0.5 |
|---|---|---|
| Clases gestoras | 1 | 3 |
| Operaciones en la clase gestora más grande | 12 | 3 |
| Atributos públicos | 9 | 0 |
| Pantallas con acceso directo a la base de datos | 4 | 0 |
| Atributos duplicados entre Recepcionista y Gerente | 4 | 0 |
