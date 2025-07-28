#Respuestas

##1a. Describa los campos que se encontrará en este tipo de archivos. ¿Qué información está allí contenida? Proporcione ejemplos.

En este tipo de archivo podemos encontrar 9 campos, los cuales son:

1. seqid: Identificador de la secuencia.
   - Puede contener caracteres como: [a-zA-Z0-9.:^*$@!+_?-|].
   - Ejemplo: ctg123 → Todos los elementos anotados en esa línea pertenecen a la secuencia "ctg123".

2. source: Fuente o software que generó la anotación.
   - Ejemplo: GenBank → Permite identificar qué herramienta hizo esa anotación.

3. type: Tipo de anotación tomado del Sequence Ontology.
   - Ejemplo: gene, mRNA, exon, CDS, TF_binding_site.
   - Indica qué tipo de elemento genómico es.

4. start: Posición inicial de la anotación.
   - Ejemplo: 1000 → Significa que comienza en la posición 1000 de la secuencia.

5. end: Posición final de la anotación.
   - Ejemplo: 9000 → Significa que termina en la posición 9000 de la secuencia.

6. score: Puntaje (valor flotante) o "." si no aplica.
   - Ejemplo: 6.2e-45 o "." → Se puede usar para filtrar anotaciones según calidad o relevancia.

7. strand: Sentido de la hebra en la que se encuentra la anotación.
   - Valores posibles:
     - "+" hebra directa
     - "-" hebra complementaria
     - "." sin información o no aplica
     - "?" desconocido
   - Ejemplo: "+" → Indica que la anotación está en la hebra positiva.

8. phase: Solo para características de tipo CDS.
   - Indica dónde comienza el siguiente codón con respecto al inicio del CDS.
   - Valores posibles: 0, 1, 2
   - Ejemplo: 0 → Significa que el codón comienza justo en el primer nucleótido del CDS.

9. attributes: Información adicional en formato clave=valor, separada por punto y coma (;).
   - Atributos comunes:
     - ID: identificador único del elemento.
     - Parent: ID del elemento del cual depende jerárquicamente (por ejemplo, un exon pertenece a un mRNA).
     - Name: nombre visible.
     - Alias: identificador alternativo o nombre secundario.
     - Dbxref: referencias cruzadas a bases de datos externas.
     - Ontology_term: término relacionado con una ontología.
     - Gap: describe alineamientos con huecos.
     - Is_circular: indica si una secuencia es circular.
   - Ejemplo:
     ID=match00003;Parent=cDNA00001;Target=mjm1123.3 1 502;Gap=M101 D1499 M401
   - Nota: Los atributos más usados en los archivos del repositorio son: ID, Name, Parent, Target y Gap.

##3a. Proporcione una breve descripción del organismo asignado en el archivo README. 
- El Vombatus Ursinus o Wombat Comun es un marsupial nativo de Australia. Viven en madrigueras, que ellos mismos excavan con sus garras y dientes. sus parientes mas cercanos son los canguros y los koalas, y Mayormente estos animales son nocturnos.
