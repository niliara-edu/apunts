# XQuery

XQuery serveix per fer consultes a un arxiu XML.

Utilitza el sistema FLOWR, que consisteix en les següents funcions:

### For

Selecciona una sequència de nodes:

#
    for $cancion in /canciones/cancion
#

## Let

Crea una nova variable, d'una manera similar a Rust:

#
    let $lanzamiento := $cancion/lanzamiento
#

## Where

Determina una condició per filtrar els resultats:

#
    where $lanzamiento < 1990
#

## Order by

Ordena els resultats.

## Return

Retorna el resultat de la consulta:

#
    return $cancion/titulo
#
