# Arrayas

- Una array es una sona de almacenamiento continuo, donde se puede introducir varios valores cada uno de ellos ubicados por la posisicion q ocupa en el array.
- Tambien son denominados arreglos o vectores, y cuando son de dos dimensiones son llamados matrices.
- Los array nos brinda la capacidad de almacenar una coleccion de elementos y acceder a ellos de manera individual.
- Cada elemento se identifica medeiante su posicion en el array, denominada **indice**
y estos indices son siempre secuenciales.
- En Javascript son altamente flexibles en terminos de los diferentes tipos de datos que podemos almacenar en cada posicion del array.

## Crear un array 

1. Declarando una array con elementos en linea 

```Javascript
let miArray = [1, 2, 3];
console.log(miArray);
```

2. Declarando un array con la sintaxis **new Array()**

```Javascript
let miArray = new Array (1, 2, 3);
console.log(miArray);
```

3. Declarando un array con un tamañano especifico utilizando la sintaxis **new Array** asignando valores despues:

```Javascript
let miArray = new Array (3);
miArray[0]= 1;
miArray[1]= 2;
miArray[2]= 3;
console.log(miArray);
```

4. Declarando un array  con elemnetos de diferentes tipos de datos



```Javascript
let miArray4 = [11, "dos", true, {nombre: "Juan", edad: 30}];
console.log(miArray4);
```

