# Intermediate - JavaScript Intermedio y Avanzado

Esta carpeta contiene conceptos intermedios y avanzados de JavaScript. Se recomienda completar la carpeta **Basic/** antes de comenzar con este contenido.

## 📋 Contenido del Curso Intermedio

### 1. Funciones Avanzadas
- **00-advanced-functions.js** - Ciudadanos de primera clase, closures, currying, callbacks, IIFE
- **01-advanced-functions-exercise.js** - Ejercicios de funciones avanzadas

**Conceptos clave:**
- Funciones como ciudadanos de primera clase
- Arrow functions avanzadas y contexto léxico `this`
- IIFE (Immediately Invoked Function Expression)
- Rest parameters (`...`)
- Spread operator
- Closures (clausuras)
- Recursividad
- Funciones parciales y currying

### 2. Estructuras de Datos Avanzadas
- **02-advanced-structures.js** - Métodos avanzados de arrays, iteradores
- **03-advanced-stuctures-execises.js** - Ejercicios de estructuras avanzadas

**Conceptos clave:**
- Métodos de arrays: map, filter, reduce, find, some, every
- Encadenamiento de métodos
- Iteradores y generadores

### 3. Objetos y Clases Avanzados
- **04-advanced-objects.js** - Object methods, property descriptors
- **05-advanced-classes.js** - Clases avanzadas, herencia múltiple, mixins
- **06-advanced-objects-classes-exercises.js** - Ejercicios de objetos y clases

**Conceptos clave:**
- Object.keys(), Object.values(), Object.entries()
- Object.assign(), Object.freeze()
- Prototipos y herencia prototípica
- Clases avanzadas
- Getters y setters avanzados

### 4. Programación Asíncrona
- **07-async.js** - Callbacks, Promises, async/await, Event Loop
- **08-async-exercise.js** - Ejercicios de programación asíncrona

**Conceptos clave:**
- Código síncrono vs asíncrono
- Event Loop (Call Stack, Web APIs, Task Queue, Microtask Queue)
- Callbacks y Callback Hell
- Promises (.then(), .catch())
- Encadenamiento de promesas
- async/await
- Manejo de errores asíncronos

### 5. APIs y Peticiones HTTP
- **09-apis.js** - Fetch API, peticiones HTTP
- **10-apis-exercise.js** - Ejercicios de APIs

**Conceptos clave:**
- Fetch API
- Métodos HTTP (GET, POST, PUT, DELETE)
- Trabajo con JSON
- Manejo de respuestas y errores
- APIs REST

### 6. Manipulación del DOM
- **11-dom.js** - Selección y manipulación de elementos DOM
- **12-dom-example.html** - Ejemplo HTML para práctica
- **13-dom-example.js** - Script de ejemplo DOM
- **14.tasklist.html** - Ejemplo de lista de tareas
- **15-tasklist.js** - Script de lista de tareas
- **16-dom-exercise.js** - Ejercicios de DOM

**Conceptos clave:**
- Selección de elementos (getElementById, querySelector, etc.)
- Manipulación de contenido y atributos
- Creación y eliminación de elementos
- Event listeners
- Delegación de eventos
- Proyecto práctico: Task List

### 7. Debugging
- **17-debugging.js** - Técnicas de debugging
- **18-debugging-exercise.js** - Ejercicios de debugging

**Conceptos clave:**
- console.log() y métodos avanzados
- Breakpoints
- Debugger statement
- Inspección de variables
- Call stack

### 8. Expresiones Regulares (RegEx)
- **19-regex.js** - Patrones, búsqueda, reemplazo
- **20-regex-exercise.js** - Ejercicios de regex

**Conceptos clave:**
- Sintaxis básica de regex
- Metacaracteres y cuantificadores
- Grupos y capturas
- Métodos: test(), match(), replace()
- Validación de datos

### 9. Testing
- **21-testing.js** - Introducción a testing
- **22-testing-test.js** - Ejemplo de tests
- **23-testing-exercise.js** - Ejercicios de testing

**Conceptos clave:**
- Fundamentos de testing
- Escribir tests básicos
- Assertions
- Test runners

## 🎯 Objetivos de Aprendizaje

Al completar esta sección, serás capaz de:

- ✅ Dominar funciones avanzadas (closures, currying, recursividad)
- ✅ Usar métodos funcionales de arrays (map, filter, reduce)
- ✅ Trabajar con programación asíncrona efectivamente
- ✅ Consumir APIs y manejar peticiones HTTP
- ✅ Manipular el DOM y manejar eventos
- ✅ Depurar código eficientemente
- ✅ Usar expresiones regulares para validación
- ✅ Escribir tests básicos

## 🚀 Cómo Usar Esta Carpeta

1. **Prerequisitos**: Asegúrate de haber completado la carpeta **Basic/** primero.

2. **Orden recomendado**: Sigue los archivos en orden numérico (00, 01, 02...).

3. **Ejecutar ejemplos JavaScript**:
   ```bash
   node 00-advanced-functions.js
   node 07-async.js
   # etc...
   ```

4. **Ejemplos DOM**: Para los archivos DOM, abre los archivos HTML en un navegador:
   - Abre `12-dom-example.html` en tu navegador
   - Abre `14.tasklist.html` para ver el proyecto de lista de tareas

5. **Practicar**: Los archivos con sufijo `-exercise.js` contienen ejercicios prácticos.

## 📝 Conceptos Destacados

### Event Loop
El Event Loop es fundamental para entender JavaScript asíncrono:
1. **Call Stack** - Pila de ejecución
2. **Web APIs** - APIs del navegador o Node.js
3. **Task Queue** - Cola de tareas (setTimeout)
4. **Microtask Queue** - Cola de microtareas (Promises)

### Promises vs Async/Await

**Promises:**
```javascript
fetch('url')
    .then(response => response.json())
    .then(data => console.log(data))
    .catch(error => console.error(error));
```

**Async/Await:**
```javascript
async function getData() {
    try {
        const response = await fetch('url');
        const data = await response.json();
        console.log(data);
    } catch (error) {
        console.error(error);
    }
}
```

### Métodos Funcionales de Arrays
```javascript
// map - transforma elementos
const doubled = [1, 2, 3].map(x => x * 2);

// filter - filtra elementos
const evens = [1, 2, 3, 4].filter(x => x % 2 === 0);

// reduce - reduce a un valor
const sum = [1, 2, 3].reduce((acc, x) => acc + x, 0);
```

## 💡 Tips de Estudio

1. **Asincronía**: La programación asíncrona puede ser confusa al principio. Practica mucho con Promises y async/await.

2. **DOM**: Abre las herramientas de desarrollo del navegador (F12) para experimentar con el DOM.

3. **APIs**: Usa APIs públicas gratuitas para practicar (JSONPlaceholder, Pokemon API, etc.).

4. **Debugging**: Aprende a usar el debugger del navegador o de Node.js, no solo console.log().

5. **RegEx**: Las expresiones regulares son poderosas pero complejas. Usa herramientas como regex101.com para practicar.

6. **Testing**: Escribir tests te ayuda a pensar en casos extremos y a escribir mejor código.

## 🛠️ Herramientas Recomendadas

- **Node.js** - Para ejecutar JavaScript fuera del navegador
- **Navegador moderno** - Chrome, Firefox, Edge (con DevTools)
- **Editor de código** - VS Code, WebStorm, Sublime Text
- **Extensiones útiles**:
  - Debugger for Chrome
  - ESLint
  - Prettier

## 📚 Proyectos Prácticos

Esta carpeta incluye ejemplos prácticos:

1. **Task List** (14.tasklist.html + 15-tasklist.js)
   - CRUD básico
   - Manipulación del DOM
   - Event handling

2. **Ejemplos de DOM** (12-dom-example.html + 13-dom-example.js)
   - Selección de elementos
   - Modificación de estilos
   - Event listeners

## 🔗 Recursos Adicionales

- [MDN Web Docs](https://developer.mozilla.org/es/docs/Web/JavaScript) - Documentación oficial
- [JavaScript.info](https://javascript.info/) - Tutorial completo
- [Eloquent JavaScript](https://eloquentjavascript.net/) - Libro gratuito

## 🎓 Certificación de Conocimientos

Para validar que has aprendido estos conceptos:

1. ✅ Completa todos los ejercicios
2. ✅ Crea un proyecto que combine: fetch API + DOM + async/await
3. ✅ Escribe tests para tu código
4. ✅ Usa debugging para encontrar y corregir errores

---

¡Sigue practicando y mejorando tus habilidades en JavaScript! 💪🚀
