# JAVA SCRIPT

## Variáveis
Variáveis são dinâmicas em JavaScript, não sendo necessário o cast de qual dataType ela armazenará, basta adicionar

```
var nomeVariavel = '';
```

### Escopo de Variáveis
Além disso as váriaveis possuem diferentes tipos de escopos, quando declaradas fora de qualquer bloco, são visíveis por todo o arquivo, e quando declaradas dentro de um bloco ela será visível apenas dentro daquele bloco.

### Declarações de Variáveis
Existem 3 maneiras de declarar uma variável em javaScript

```
var variavel = ''; 
let variavel = ''; 
const variavel = ''; 
```

### Var
Utilizada em todos os escopos, geralmente no global, é a maneira genérica de declarar uma variável, sem limites de alteração.

### Let
Por convenção utilizado para escopo local, onde a variável será utilizada sommente naquele bloco de código

### Const
Utilizada para declarar constantes imutáveis que serão utilizadas no bloco de código

---

### Diferentes tipos de comparação
- "==" Realiza a comparação comum, comparando o valor da variável

```
"0" == 0;
```

- "===" Realiza a comparação por meio do dataType, então a comparação anterior retorna true, ja que estamos comparando os valores, caso realizamos a mesma comparação porém com o === retornará false pois estamos comparando os dois dataTypes

```
"0" === 0;
```
