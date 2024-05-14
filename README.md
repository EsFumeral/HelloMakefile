# Projecte hellomake

Un hello world escrit en C per a practicar
GNU Makefile

## Llegiu les instruccions amb atenció

### Requeriments

gcc instal·lat

```bash
gcc --version

```

## Inici

1. Assegurau-vos de tenir una carpeta amb nom C a la ruta $HOME/Proyectos

```bash
cd $HOME/Proyectos
mkdir C
cd C
```

2. Posau nom al vostre projecte: HelloMake

```bash
mkdir HelloMake
cd HelloMake
```


## README

Afegiu aquest fitxer README.md a la carpeta $HOME/Proyectos/C/HelloMake


## Llicència

Es important tenir una llicència vàlida per al projecte. 

```bash
touch LICENSE
```


Copiau el text


```
Copyright <YEAR> <COPYRIGHT HOLDER>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

I aferrau lo a un document amb nom LICENSE

# Creau els fitxers de codi.


```bash
touch hellomake.h
```
Aferrau el codi

```C
/* 
Cabecera de ejemplo
*/


void myPrintHelloMake(void);
```



```bash
touch hellomake.c
```
Aferrau el codi

```C
#include "hellomake.h"

int main() {
    // llama otra función
    myPrintHelloMake();
    return(0);
}


```


```bash
touch hellofunc.c
```

Aferrau el codi

```C
#include "hellomake.h"
#include <stdio.h>

void myPrintHelloMake(void) {
    printf("Hello makefiles!\n");
    return;
}

```

## Construim el makefile


```bash
touch Makefile
```

Aferrau el codi

```Makefile

hellomake: hellomake.c hellofunc.c
     gcc -o hellomake hellomake.c hellofunc.c -I.


```

## Compilam

```bash
make
./hellomake
```

Presentau la carpeta HelloMake comprimida a la tasca.
