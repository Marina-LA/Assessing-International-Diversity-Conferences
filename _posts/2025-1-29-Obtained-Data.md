---
layout: post
title: "Obtained Data"
permalink: /obtained-data
post-image: "/assets/images/Decoration/Top_Drawing.png"
description: In this section, statistics of the data collected for the study will be shown.
---

Para realizar este estudio se han obtenido papers a partir del año 2012 hasta el 2023. Estos papers pertenecen a 10 conferencias distintas (NSDI, SoCC, Middleware, EuroSys, ICDCS, CCGRID, Euro-Par, SIGCOMM, IEEE Cloud y IC2E). A continuación, se mostrará más en detalle la cantidad de datos que se ha recolectado para los accepted papers, las citas y los miembros del Program Committee.

# Accepted Papers

Los accpeted papers son los papers que han sido publicados en cada una de las conferèncias. Estos datos se han obtenido mediante el crawler. En total se han obtenido 6800 papers publicados entre los 11 años estudiados de las 10 conferencias. La tabla que se muestra a continuación detalla el numero de papers que se han obtenido para cada una de las conferencias en cada uno de los 10 años estudiados.

// TAULA NUMERO PAPERS

## Accepted Papers Missing Data

Aunque en la gran mayoria de los casos se ha conseguido obtener todos los datos necesarios de los accepted papers, se han dado situaciones donde obtener algunos de estos datos no ha sido posible. En consequencia, al realizar la asignacion de un paper a un continente, hay papers donde esta asignacion no se ha podido realizar por falta de datos. En la tabla que se muestra a continuación se datalla el porcentaje de papers de cada conferencia que no tienen ningún continente asignado, por lo que en los analisis realizados posteriormente dicho porcentaje de papers no se tendra en cuenta.

// TAULA % MISSING PAPERS

# Citations

Para este estudio hemos considerado los cited papers como cualquier documento que se haya citado o referenciado en un los accepted papers de las conferencias. Por este motivo no simplemente estamos hablando de papers de conferencias, sino que también podemos encontrar articulos de revistas, libros, etc.
En total se han obtenido 160666 datos de citas entre todos los accepted papers de las 10 conferencias. En la tabla que se muestra a continuación se pueded observar de forma detallada el nuemro de datos de citas que se han obtenido para cada uno de los años en las 10 conferencias estudiadas. Cabe destacar que hay datos de citas que se pueden estar contando dos veces, al ser citados en distintos años y distintas conferèncias. Sin embargo, para los analisis realizados, los papers que se repiten dentro de una misma conferencia en distintos años solo han sido contados una sola vez.

// TAULA DE PAPERS CITATS

## Citations Missing Data

Tal y como se ha observado, hay una gran cantidad de datos referntes a las citas, por lo que obtener información de cada uno de estos ha sido muy complicado. A consequencia de esto, el porcentage de datos de citas sin los datos necesarios para poder realizar el posterior analisis es muy elevado.
Para mitigar este problema, hemos aplicado dos estrategias distintas.

### First Approach

Primero intentamos que el numero de accepted papers sin datos de citas fuera menor al 10%. En la mayoria de las conferencias se puedo cumplir este requisito, menos en una, NSDI. Para poder solucionar esto optamos por no incluir los papers de distintos años, intentando que el numero de accepted papers que no tubieran información repecto a los años  fuera menor del 10%.
Es por esto que se excluyeron los accepted papers de los años 2014, 2015 y 2022 de NSDI para los analisis de las citas.

Después de realizar este cambio, el numero de datos de citas del que se dispuso fue de 124228. Assumiendo todos estos datos de citas, el porcentage de citas que no disponen de la suficiente información para realizar los analisis deseados sigue siendo muy elevado. En la tabla que se muestra a continuación se pueden ver dichos porcentages para cada una de las 10 conferencias.

// TAULA MISSING CITATIONS

### Second Approach

Tal y como se observa en la tabla anterior, el porcentage de datos de citas sin la suficiente información necesaria sigue siendo muy elevado (más de un 30% en varias conferencias), por lo que optamos por estudiar la distribución de los datos en una pequeña muestra de datos sin información.

Lo que decidimos realizar fue lo siguiente:

1. Se escogio al azar una muestra del 10% de los datos de citas que no cumplian con los requisitos. Es decir, datos de citas sin la información necesaria para realizar el estudio. Solo se realizo esto para el año 2023 de las conferencias de NSDI y ICDCS.
2. Para este 10% de los datos se obtuvo la información necesaria de forma manual.
3. Se analizo la distibución de dichos datos usando el metodo de Chi-Square Godness-of-Fit para evaluar si los datos seguian una distribución parecida.

Los datos obtenidos mostraron que esta pequeña muestra de datos si seguia la distribución esperada (la distribución que siguen el resto de los datos de los cuales si se tiene información), por lo que determinamos que los resultados obtenidos en los analisis de las citas son validos pese al pequeño inconveniente de datos faltantes, ya que incluso si dispusieramos de dichos datos, el resultado seguiria la misma distribución.

# Program Committee

La obtención de los datos del program committee ha sido más complicada, siendo posible automatizarla, se ha realizado de forma manual. En consequencia, pueden existir pequeños errores en dichos datos fruto del error humano. No obstante, dichos datos han sido revisado numerosas veces para reducir estos errores.
Otro problema con el que nos hemos encontrado al obtener estos datos es que en ciertos casos ha sido imposible obtener ninguna información sobre el program committee de una conferencia en un cierto año.
En total, se ha obtenido un total de 12147 miembros del program committee. En la tabla que se muestra a continuación se puede observar de forma más detallada el nuemro de miembros del program committee obtenidos para cada una de las conferencias.

// TAULA PC MEMBERS

## Committee Members Missing Data

Para algunos de los miembros del program committee ha sido imposible obtener toda la información necesaria para realizar los analisis desados. 

// TAULA MISSING PC MEMBERS