# Prediccion_vuelos_santiago_de_chile
 
Autor:

Juan Camilo Macías Betancur Data Analyst | Data Scientist

Abstracto:

● El problema que se trata de resolver es predecir la probabilidad de atraso de los vuelos que aterrizan o despegan del
aeropuerto de Santiago de Chile (SCL). Para eso utilizó un dataset de datos públicos y reales donde cada fila
corresponde a un vuelo que aterrizó o despegó de SCL. También se utilizó un dataset del estado del clima durante el periodo analizado.
● Para cada vuelo se cuenta con la siguiente información:
- Fecha-I: Fecha y hora programada del vuelo.
- Vlo-I: Número de vuelo programado.
- Ori-I: Código de ciudad de origen programado.
- Des-I: Código de ciudad de destino programado.
- Emp-I: Código aerolínea de vuelo programado.
- Fecha-O: Fecha y hora de operación del vuelo.
- Vlo-O: Número de vuelo de operación del vuelo.
- Ori-O: Código de ciudad de origen de operación
- Des-O: Código de ciudad de destino de operación.
- Emp-O: Código aerolínea de vuelo operado.
- DIA: Día del mes de operación del vuelo.
- MES: Número de mes de operación del vuelo.
- AÑO: Año de operación del vuelo.
- DIANOM: Día de la semana de operación del vuelo.
- TIPOVUELO : Tipo de vuelo, I =Internacional, N =Nacional.
- OPERA: Nombre de aerolínea que opera.
- SIGLAORI: Nombre ciudad origen.
- SIGLADES: Nombre ciudad destino.

● Generación de columna adicionales:

- Temporada_alta: 1 si Fecha-I está entre 15-Dic y 3-Mar, o 15-Jul y 31-Jul, o 11-Sep y 30-Sep, 0 si
no.
- dif_min: diferencia en minutos entre Fecha-O y Fecha-I.
- atraso_15: 1 si dif_min > 15, 0 si no.
- periodo_dia: mañana (entre 5:00 y 11:59), tarde (entre 12:00 y 18:59) y noche (entre 19:00 y 4:59),
en base a Fecha-I.
