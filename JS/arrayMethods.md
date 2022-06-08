# Bucles y Metodos de Arreglos Modernos en JS

Este es un resumen de estudio/aprendizaje algunos _casos de uso_ de _Bucles y Metodos arreglos modernos en JavaScript_, comparando php, JSTradicional, JSModerno (o ES6).

A partir del video y los conocimientos obtenidos hasta el momento. Enfatizando dudas comunes [Creditos](#creditos)

---

## Tabla de Contenidos

- [Metodos](#Metodos)

  - [Map](#map)
  - [Filter](#filter)
  - [Find](#find)
  - [FindIndex](#findIndex)
  - [Reduce](#reduce)
  - [Every](#every)
  - [Some](#some)
  - [Include](#include)
  - [Sort](#sort)

- [Creditos](#creditos)

---

## Metodos

### Map

hacer _una operacion_ por _cada elemento_ de **un** arreglo,
y _**guardar** valores actualizados_ en **otro** arreglo

```javascript
let arr = ["juan", "marcos", "lena", "sergio"];
```

```javascript
//JST
let result = [];

for (let index = 0; index < arr.length; index++) {
  const item = arr[index];

  result.push("<div>${item}</div>");
}
console.log(result); //['<div>juan</div>','<div>marcos</div>','<div>lena</div>','<div>sergio</div>',]
```

```javascript
//ES6

let result2 = arr.map((item, index) => {
  return `<div>${item}</div>`;
});

console.log(result2); //['<div>juan</div>','<div>marcos</div>','<div>lena</div>','<div>sergio</div>']
```

### Filter

hacer _un filtro_ de _cada elemento_ de **un** arreglo
_basado en una condicion_
y _**guardar** todas las coincidencias_ en **otro** arreglo

```javascript
let arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16];
```

```javascript
//JST
let result = [];

for (let index = 0; index < arr.length; index++) {
  const item = arr[index];

  if( item >= 5 && item <= 11;){
      result.push(item);
  }

}
console.log(result); //[5,6,7,8,9,10,11]
```

```javascript
//ES6

//usando una funcion tradicional

let result2 = arr.filter(function (item, index) {
  return item >= 5 && item <= 11;
});

console.log(result2); //[5,6,7,8,9,10,11]

//usando una funcion flecha

let result2 = arr.filter((item, index) => item >= 5 && item <= 11);

console.log(result2); //[5,6,7,8,9,10,11]

// ..como no estoy utilizando la variable index podria dejar de utilizarla y sacar los ()
```

### Find

hacer _un filtro_ de _cada elemento_ de **un** arreglo
_basado en una condicion_
y _**obtener el indice** de la **primera** coincidencia_

```javascript
let arr = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16];
```

```javascript
//JST
let result = [];

for (let index = 0; index < arr.length; index++) {
  const item = arr[index];

  if( item >= 5 && item <= 11;){
      result.push(item);
  }

}
console.log(result); //[5,6,7,8,9,10,11]
```

```javascript
//ES6

//usando una funcion tradicional

let result2 = arr.filter(function (item, index) {
  return item >= 5 && item <= 11;
});

console.log(result2); //[5,6,7,8,9,10,11]

//usando una funcion flecha

let result2 = arr.filter((item, index) => item >= 5 && item <= 11);

console.log(result2); //[5,6,7,8,9,10,11]

// ..como no estoy utilizando la variable index podria dejar de utilizarla y sacar los ()
```

### FindIndex

### Reduce

### Every

### Some

### Include

### Sort

---

## Notas

Notas sobre bucles

1. Inicializacion de la variable
2. Condicion de Permanencia
3. La variable que controla la condicion de iteracion
4. Codigo a ejecutar mientras se cumpla 2

Caso de Uso: Tengo _valores en un arreglo [1]_ y _**necesito** hacer algo con ellos [4]_ en _determinado contexto [2, 3]_

```php
//php
for (variable; condicion; incremento ) { //for (1; 2; 3 ){4}
    //codigo a ejecutar
}
```

```php
//php

while (variable>0) {
    echo $contador;
    $contador --;
}
// si la condicion no es false en algun momento -> 8loop

```

```php
//php

do {
    echo $cantidad;
    $cantidad --;
} while ($cantidad>0);

// ejecuta por lo menos unas vez el codigo y si la condicion while **es** o *se vuelve* false, no se ejecuta mas

```

---

## Creditos

[MÉTODOS DE ARREGLOS MODERNOS EN JAVASCRIPT](https://www.youtube.com/watch?v=bkgXlQp5hbI)

```

```
