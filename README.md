# Ejercicio: Testing de una Calculadora con Jest

## Explicación

En este ejercicio, crearemos una simple calculadora con las funciones básicas de suma, resta, multiplicación y división usando JavaScript. Luego, verificaremos el correcto funcionamiento de las funciones utilizando pruebas unitarias. Para nuestras pruebas usaremos Jest, un potente framework de pruebas para JavaScript.

Las funciones de la calculadora serán las siguientes:

- isNumber(a): Asume que a es un número. Si es así, devuelve true. Si no, devuelve false.
- add(a, b): Asume que a y b son números. Si no es así, lanza un error. Si es así, devuelve la suma de a y b.
- subtract(a, b): Asume que a y b son números. Si no es así, lanza un error. Si es así, devuelve la resta de a y b.
- multiply(a, b): Asume que a y b son números. Si no es así, lanza un error. Si es así, devuelve el producto de a y b.
- divide(a, b): Asume que a y b son números y que b no es 0. Si no es así, lanza un error. Si es así, devuelve la división de a entre b.

## Paso 1: Configuración del proyecto

Primero, necesitamos configurar nuestro proyecto. En la terminal, ejecutamos:

```
npm init -y
npm install --save-dev jest
```

Después, agregamos la siguiente línea en tu archivo `package.json` en la sección "scripts":

```json
"scripts": {
    "test": "jest"
}
```

## Paso 2: Creación del archivo con las funciones de la calculadora

Crea un archivo `calculator.js` que contendrán las funciones de la calculadora.

## Paso 3: Creación del archivo de pruebas

Crea un archivo `calculator.test.js`, que será donde escribiremos nuestras pruebas unitarias para las funciones que definiremos en `calculator.js`.

## Paso 4: Escribir y ejecutar los tests

Para cada función, haremos las pruebas correspondiente en un mismo grupo. Para ello usaremos el método `describe` de Jest. Dentro de cada grupo usaremos `it` o `test`. Para cada cosa que queramos comprobar usaremos expect(<expresión>).<método>(<resultado_esperado>). Donde podemos usar métodos como `toBe`,`toEqual`,`not`, `toThrow`, etc.

Si símplemente se busca comprobar si se lanza una excepción, se puede usar el método `toThrow` sin pasarle ningún parámetro.

Para ejecutar las pruebas, puedes usar el siguiente comando en la terminal: `npm test`. Si todo va bien, deberías ver un mensaje en tu terminal que indica que todas las pruebas pasaron con éxito. Si alguna prueba no pasa, obtendrás un mensaje de error que te indicará qué prueba falló y por qué.

## Recursos

- [Jest](https://jestjs.io/docs/getting-started)
