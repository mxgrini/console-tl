# console-lt (Console Log Time)

## Description

A Console that emits logs with date and time

See the documentation: [/docs](https://leydev.github.io/console-tl/)

## Install and use

Instalation:   
```
bash: npm i console-lt
```
Use:   
```
const consoleLT = require('console-lt')

consoleLT.log('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [LOG]: Hello Wolrd
consoleLT.info('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [INFO]: Hello Wolrd
consoleLT.warn('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [WARN]: Hello Wolrd
consoleLT.error('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [ERROR]: Hello Wolrd
```

With method "overwrite", the default console global will be overwriten. So you can use global console to log with date and time:   

```
require('console-lt').overwrite()

console.log('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [LOG]: Hello Wolrd
console.info('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [INFO]: Hello Wolrd
console.warn('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [WARN]: Hello Wolrd
console.error('Hello Wolrd') //Output: 2020-02-13 14:01:23.234 [ERROR]: Hello Wolrd
```

**Last update: 21/02/2020**  
- Método overwrite().

**update: 13/02/2020**  
- Criação do módulo;
- Método log();
- Método info();
- Método warn();
- Método error().