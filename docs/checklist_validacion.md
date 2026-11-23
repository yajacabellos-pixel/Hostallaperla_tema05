# Checklist de validación del modelo (v0.5)

| N.° | Criterio | Resultado | Observación |
|---|---|---|---|
| 1 | Nomenclatura uniforme | Cumple | Todo en español y sin tildes en el modelo |
| 2 | Asociaciones con multiplicidad | Cumple | 7 relaciones revisadas |
| 3 | Toda clase tiene al menos un requisito | Cumple | Ver matriz/matriz_requisito_clase.csv |
| 4 | Todo requisito tiene al menos una clase | Cumple | RF01–RF09, RNF01, RNF02 |
| 5 | Sin redundancias | Cumple | Corregido con R3 y R4 |
| 6 | Visibilidad indicada | Cumple | Atributos privados, operaciones públicas |
| 7 | Paquetes sin ciclos | Cumple | Dominio no depende de otros paquetes |
| 8 | Mensajes de secuencia existen como operaciones | Cumple | CU01 y CU05 |
| 9 | Enumeraciones modeladas | Parcial | Falta dibujarlas como <<enumeration>> |
| 10 | Seguridad de la clave | Pendiente | Guardar solo un hash de la clave |
