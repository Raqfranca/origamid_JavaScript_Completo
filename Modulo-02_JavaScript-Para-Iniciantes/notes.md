### **Variáveis** 

**Responsáveis por guardar dados na memória.** 

Inicia com a palavra var, let ou const

var nome = 'André';
let idade = 28;
const possuiFaculdade = true;

**Evitam repetições**

- Conceito de DRY (Don't repeat yourself)

var preco = 20;
var totalComprado = 5;
var precoTotal = preco * totalComprado;

**Sintaxe**

Palavra chave var seguida do nome, sinal de igual e o valor.

var nome = 'André';
var idade = 28;
var possuiFaculdade = true;

**Vírgula**

A vírgula pode ser utilizada para criar mais de uma variável, sem repetir a palavra chave var.

var nome = 'André',
    idade = 28,
    possuiFaculdade = true;

**Sem valor**

Pode declarar ela e não atribuir valor inicialmente.

var precoAplicativo;
// retorna undefined

**Hoisting**

São movidas para cima do código, porém o valor atribuído não é movido.

console.log(nome);
var nome = 'André';
// Retorna undefined

Fica igual a:

var nome 
console.log(nome);
var nome = 'André';

o console.log retorna = undefined

**Mudar o valor atribuído**

É possível mudar os valores atribuídos a variáveis declaradas com var e let. Porém não é possível modificar valores das declaradas com const

var idade = 28;
idade = 29;

let preco = 50;
preco = 25;

const possuiFaculdade = true;
possuiFaculdade = false;
// Retorna um erro
