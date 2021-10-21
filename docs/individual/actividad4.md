# JSON & XML

## JSON

!["JSON_ejemplo"](/archivos/actividad4/jsonExample.jpg)

JSON (JavaScript Object Notation) es un **formato ligero de intercambio de datos**. JSON es de fácil lectura y escritura para los usuarios. Leerlo y escribirlo es simple para humanos, mientras que para las máquinas es simple interpretarlo y generarlo. Está basado en un subconjunto del Lenguaje de Programación JavaScript, Standard ECMA-262 3rd Edition - Diciembre 1999.

JSON es un **formato de texto que es completamente independiente del lenguaje** pero utiliza convenciones que son ampliamente conocidos por los programadores de la familia de lenguajes C, incluyendo C, C++, C#, Java, JavaScript, Perl, Python, y muchos otros.

Está constituído por:

- Una colección de pares de nombre/valor. En varios lenguajes esto es conocido como un objeto.
- Una lista ordenada de valores. En la mayoría de los lenguajes, esto se implementa como arreglos, vectores, etc.

### Caracteristicas

Sus principales características son:

- JSON es solo un formato de datos.
- Requiere usar comillas dobles para las cadenas y los nombres de propiedades. Las comillas simples no son válidas.
- Puede tomar la forma de cualquier tipo de datos que sea válido para ser incluido en un JSON, no solo arreglos u objetos.

### Usos

- Su principal uso radica en el procesamiento de datos y al no depender de ningun lenguaje de programación este mismo puede ser implementado en cualquier programa.
Su sencillez le ha permitido posicionarse como alternativa a XML.

## Ejemplos
- Datos de un rpg
```json
{
  "player1": {
    "hp": 10,
    "dmg": 1,
    "type": "fire"
  },
  "player2": {
    "hp": 5,
    "dmg": 3,
    "type": "air"
  }
}
```

- Datos de una cuenta
```json
{
  "name": [
    "Claudio",
    "Hassiel"
  ],
  "last_names": [
    "Araujo",
    "Palestina"
  ],
  "money": 30.5,
  "isAdmin": true
}
```

- Horario de clase
```json
{
  "lunes": {
    "ingles": [
      7,
      9
    ],
    "optimizacion": [
      9,
      11
    ]
  },
  "martes": {
    "ingenieria": [
      7,
      9
    ],
    "estadistica": [
      11,
      1
    ]
  },
  "miercoles": {
    "optimizacion": [
      9,
      11
    ],
    "estadistica": [
      11,
      1
    ]
  }
}
```

## XML

!["XML_ejemplo"](/archivos/actividad4/xmlExample.png)

Extensible Markup Language (Lenguaje de Marcado Extensible) es una especificación de W3C como lenguaje de marcado de propósito general. Esto significa que, a diferencia de otros lenguajes de marcado, XML **no está predefinido**, por lo que debes **definir tus propias etiquetas**. El propósito principal del lenguaje es **compartir datos** a través de diferentes sistemas, como Internet.

- XML es un subconjunto de SGML(Estándar Generalised Mark-up Language),simplificado y adaptado a Internet
- XML es un meta-lenguaje que nos permite definir lenguajes de marcado adecuados a usos determinados.
- No es una versión mejorada de HTML
- HTML es una aplicación de SGML por lo tanto de XML

### Características

Sus principales características son:

- Es un subconjunto de SGML que incorpora las tres características más importantes de este:
    * Extensibilidad
    * Estructura
    * Validación
- Orientado a los contenidos no a la presentación
- Etiquetas definidas por el usuario para crear los documentos

### Usos

- Documentos: Similar a HTML, este puede ser usado para crear documentos con la excepción de que XML soporta mas elementos.
- Intercambio de datos: Para intercambiar información entre humano/maquina, se usa mas bases de datos por Internet, pues su extensibilidad le permite ajustarse a las necesidades de cualquier aplicación

## Ejemplos

- Datos de un rpg
```xml
<?xml version="1.0" encoding="UTF-8"?>
<root>
   <player1>
      <dmg>1</dmg>
      <hp>10</hp>
      <type>fire</type>
   </player1>
   <player2>
      <dmg>3</dmg>
      <hp>5</hp>
      <type>air</type>
   </player2>
</root>
```

- Datos de una cuenta
```xml
<?xml version="1.0" encoding="UTF-8"?>
<root>
   <isAdmin>true</isAdmin>
   <last_names>
      <element>Araujo</element>
      <element>Palestina</element>
   </last_names>
   <money>30.5</money>
   <name>
      <element>Claudio</element>
      <element>Hassiel</element>
   </name>
</root>
```

- Horario de clase
```xml
<?xml version="1.0" encoding="UTF-8"?>
<root>
   <lunes>
      <ingles>
         <element>7</element>
         <element>9</element>
      </ingles>
      <optimizacion>
         <element>9</element>
         <element>11</element>
      </optimizacion>
   </lunes>
   <martes>
      <estadistica>
         <element>11</element>
         <element>1</element>
      </estadistica>
      <ingenieria>
         <element>7</element>
         <element>9</element>
      </ingenieria>
   </martes>
   <miercoles>
      <estadistica>
         <element>11</element>
         <element>1</element>
      </estadistica>
      <optimizacion>
         <element>9</element>
         <element>11</element>
      </optimizacion>
   </miercoles>
</root>
```

## Comparativa

| JSON | XML |
| --- | --- |
| Facil de entender | Facil de entender |
| Puede resultar confuso | Formato estricto |
| Mas facil de leer que XML | Analisis sintáctico facil |
| No extendible | Extendible |
| Procesado rapido | Procesado lento |

## Fuentes
1. https://www.mundolinux.info/que-es-xml.htm
2. https://www.ibm.com/docs/es/baw/20.x?topic=formats-javascript-object-notation-json-format
3. https://www.json.org/json-es.html