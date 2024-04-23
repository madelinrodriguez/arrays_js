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

## Acediendo a la informacion de un Array

### Propiedad length
- Devuelve la cantidad de elemntos de la array

### Operador [pos]
- Permite aceder para leer  o modificar  en el elemeto pos de  array

### Metodo at(pos)
- Devuelve el elmento de la posicion pos. El parametro admite valores negativos  lo que significa que empieza a contar por el final del array.

```Javascript
const letters = ["A", "B", "C"];
console.log(letters.length); 
console.log(letters[2]);
console.log(letters[5]);
```

## Añadir o eliminar elementos 
- Push(ele1, ele2): añade uno o varios elementos al final del array. Devuelve el tamaño del array.

```Javascript
let miArray =[1, 2, 3,];
miArray.push(4);  // Agrega el elemento 4 al final del array
console.log(miArray);
```
- pop():  Devuelve el ultimo elemento del array y loelimina 

```Javascript
let miArray =[1, 2, 3,];
miArray.pop(4);  //Eliina el ultimo elemento del array
console.log(miArray);
```

- unshift(ele1, ele2);
uno o varios elemntos al inicio, devolviendo el tamaño del array despues de añadidos 

```Javascript
let miArray =[1, 2, 3,];
miArray.unshift(0);  //Agrege el elemento 0 al inicio del array
console.log(miArray);
```

-shift(): devuelve el primer elemneto del array y lo elimina

```Javascript
let miArray =[1, 2, 3,];
miArray.unshift(0);  //Elimina el primer elemeno del array
console.log(miArray);
```

- concat(ele1, ele2): concatena dos array 

```Javascript
let miArray =[1, 2, 3,];
let miOtroArray =[4, 5];
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(nuevoArray);
```

-split(separador): a partir de una cadena, crea un array dividiendo dicha cadena en elemntos delimitados por separador 

```Javascript
let miString="Hola, ¿como estas?";
let miArray = mistring.split(" ");
console.log(miArray);
```

-join(separador): a partir de un array, crea una cadena separando cada elemento con el separador.

```Javascript
lt miArray= ["Hola", "¿como", "estas?"];
let miArray = miArray.join("  ")
console.log(miString);
```

## Busqueda de elementos en una arrasy

- includes(elementos): devuelve true o false si el elemento existe o no dentro del array
- indexOf(elemnto): devuelve la posicion de la primera aparicion del elemneto. si no existe, devuelve -1.
- lastIndexOf(elemto): devuelve la posicion de la ultima apracicion del elemnto. si no exiate devuleve -1.

## Modificar el array o crearr frangmentos
- slice(inicio, fin): devuelve un array con los elementos desde la posicion inicio hasta la posicion fin, ambos excluidos.

## Ordenar elemntos de una array 
-reverse(): invierte el orden de los elementos del array
- sort():  ordena el array alfabeticamente 
-sort(criterio): ordena el array con el criterio determinado por la funcion criterio.

## Borra elementos de una array
- se puede borrar el contenido de un elemneto de una array poniendo su valor a null o sagnando una cadena basida 
- para eliminar complteamente un elemento de la array se utiliza el operador delete.

## recorido de una array
1. recorrer con un blucle clasico pasado por todos los elmentos

```Javascript
var diad =["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"]
for(i=0;i<dias.leng;i++)
{
    console.log(dias[i]);

}
```

2. recorrer con un while, pasado por todo loes elemntos.

```Javascript
var diad =["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"]
var i=0;
while(i<dias.length)
{
    console.log(dias[i]);
    i++;
}
```

3.usando la sentecia for..in.

```Javascript
var diad =["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"]
for(let index in dias)
{
    console.log(dias[index]);
    
}
```
## array multidimensionales

. recorrer con un while, pasado por todo loes elemntos.

```Javascript
const matrix =[
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
```
- recorer una matris utilizando bucles animados

```Javascript
var diad =["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"]
for(let i=0;i<matriz-length;i++)
    for(let j=8;matriz[i].length;j++)
{
    console.log(matriz[i][i]);
    
}
```


# Ejecicios 
1. dada una lista de numeros separados por coma, clacular la suma, el mayor, el menor y la media de todos.

2. introducir dos cadenas con elemntos separados por coma, y con un boton concatenar las dos cadenas y mostrarlas en la pantallla.

3.  introducir uno a uno los elemenytos en un array a travez de un boton. con otro boton se va a eliminando el ultimo lemento. siempre que se pulce alguno de los botones de debe mostrar el contenido del array.

4. introduce u cojunto de numeros separados por comas. cuando se pulsa el boton "pares" cargar una tabla con los numeros introducidos y luego crear otra que solo incluya los numeros pares y mostrarla.