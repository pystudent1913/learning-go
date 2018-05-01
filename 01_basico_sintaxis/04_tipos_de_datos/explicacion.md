# [Referencia] (https://golang.org/ref/spec#Types)

- Booleano ->  true/false
- Numerico
    - uint(8|16|32|64): numero sin signo (aprox 0 to 2x9x10^20)
    - int(8|16|32|64): enteros (aprox -9x10^20 to +9x10^20)
    - float(32|64): numero de punto flotante (decimales)
    - complex(64|128): numeros imaginarios
    - byte: alias para uint8
    - rune: alias para  int32


- En go debes ser exacto al momento de sumar variables
    - puedes sumar: int + int
    - pero no: int8 + int || int8 + int16 || ... etc ...

    - asi que en todo caso debes castear(cambio TEMPORAL de una variablen)
     ```go
     <tipo-de-dato-a-cambiar>(<variable>)
     ```
     OJO: tomar en cuenta las restricciones del tipo de dato como int8|16|32|64 tienen diferentes limites
    - prioridad aritmetica (  * / + - )


- Para formear un texto se usa:
    ```go
     Printf("hola $uno $dos", uno, dos)
    ```
- Y para ver el tipo de una variable
    ```go
    fmt.Printf("var es de tipo: %T", var)
    ```