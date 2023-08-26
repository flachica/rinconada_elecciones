# Resultados electorales en La Rinconada desde 1977

Datos procedentes de la web del Ministerio del Interior https://infoelectoral.interior.gob.es/opencms/es/elecciones-celebradas/area-de-descargas/
Tratados de forma automatizada para agrupar las distintas candidaturas y poder sacar indicadores y gráficas

## Fichero: Partido (party).csv

Listado de partidos. Cada candidatura se repite pues cada una de ellas se ha obtenido en un proceso electoral (legislatura) diferente. El esquema de datos del Ministerio no ofrece un identificador único general.


## Fichero: Grupo de partidos (party.group).csv

Nombre de los grupos de partidos. La edición y la inclusión de los partidos ha sido manual por el autor. 

summary_type: Rinconada -> Los grupos son creados para obtener el porcentaje de votos obtenidos en la localidad
              Sevilla -> Los grupos son creados para obtener el porcentaje de votos obtenidos en la provincia
              Andalucía -> Los grupos son creados para obtener el porcentaje de votos obtenidos en la comunidad autónoma
name: ABS -> Abstención en La Rinconada. Grupo que representa el porcentaje de abstención
      IT -> Izquierda tradicional. Grupo formado por el PSOE principalmente
      IA -> Izquierda alternativa. Grupo formado por el PCE, IU o Podemos
      DER -> Derecha. Grupo formado por la UCD/CDS, AP, PP, Cs, etc

## Fichero: Legislatura (legislature).csv

Elecciones municipales o al congreso

Año comienzo: Año en el que se celebran las elecciones
Mes comienzo: Mes de las elecciones
Tipo de elección: Municipales o Congreso
Población
Votos: Votos totales (nulos y blancos incluidos)
Votos en blanco
Votos nulos
Votos válidos: Votos dirigidos a candidaturas

## Fichero: Resultados planos (plain.result.abs.party).csv

Expresa el porcentaje de votos de cada partido y grupo de partidos

legislature_id: Identificador de legislatura
party_group_id: Identificador de grupo de partidos
party_id: Identificador de partido
percentaje: Porcentaje de votos (el más alto incluye el voto en blanco según la norma electoral)
votes: Votos obtenidos

## Fichero: Plain Result (plain.result.abs.diff).csv

Expresa la diferencia de porcentaje del electorado de La Rinconada respecto de la provincia o la autonomía

legislature_id: Identificador de legislatura
summary_type: Sevilla -> Grupo para expresar la diferencia de porcentaje entre el grupo del mismo nombre a nivel local menos el de nivel provincial
party_group_id: Identificador de grupo de partidos
diff_percentaje: Diferencia de porcentaje

