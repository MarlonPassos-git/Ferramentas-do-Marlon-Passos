
# Como funciona 
Nos exemplos voce vera, ou uso do sifrão e mais um numero `$1`, ele representa a ordem dos tabs no seu código. Se o mesmo simbolo aparece repetido, significa que oque for escrito ali vai se refletir para o outro lugar.

Na minha cabeça as os Snippets deveria refletir a primeira inicial de cada palavra de como escrevemos o codigo, ou como a frase soa.

Onde estiver recrito "fileName" significa que o snippet pego o nome do arquivo e adicionou ao contexto. Ate a formatação de maiusculo e minusculo vai ser levado em consideração.

Quando acontece uma situção de declaração de tipagem e uso ao mesmo tempo o valor da tipagem de uso vai ser ajustada automatimente depois do TAB

# Referencia 


## Console

### ``clg`` 
language: ``*.js`` | ``*.ts`` | ``*.tsx`` | ``*.jsx``

```js
console.log($1);
```

## Funções 

### ``f``
language: ``*.js`` | ``*.ts`` | ``*.tsx`` | ``*.jsx``
```ts
function $1($2) {
  $3
}
```

### ``af``
language: ``*.js`` | ``*.ts`` | ``*.tsx`` | ``*.jsx``
```ts
async function $1($2) {
  $3
}
```

### ``ef``
language: ``*.js`` | ``*.ts`` | ``*.tsx`` | ``*.jsx``
```ts
export function fileName($1) {
  $2    
}

```

### ``eaf``
language: ``*.js`` | ``*.ts`` | ``*.tsx`` | ``*.jsx``
```ts
export async function fileName($1) {
  $2    
}
```

### ``edf``
language: ``*.js`` | ``*.ts`` | ``*.tsx`` | ``*.jsx``
```ts
export default function fileName($1) {
  $2    
}
```

### ``edaf``
language: ``*.js`` | ``*.ts`` | ``*.tsx`` | ``*.jsx``
```ts
export default function fileName($1) {
  $2    
}
```

### ``efwot``
language: ``*.ts`` | ``*.tsx``
```ts
type IFileName = {
  $1  
}

export function fileName({
  $1
}: IFileName) {
  $2
}
```

### ``eafwot``
language: ``*.ts`` | ``*.tsx``
```ts
type IFileName = {
  $1  
}

export async function fileName({
  $1
}: IFileName) {
  $2
}
```

### ``edfwot``
language: ``*.ts`` | ``*.tsx``
```ts
type IFileName = {
  $1  
}

export default function fileName({
  $1
}: IFileName) {
  $2
}
```

### ``edafwot``
language: ``*.ts`` | ``*.tsx`` 
```ts
type IFileName = {
  $1
}

export defalt async function fileName({
  $1
}: IFileName) {
  $2
}

```