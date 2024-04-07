## Exercicios em Java Script

#### 1. Variáveis
Crie 5 variáveis e atribua valores, respeitando os tipos de dados a serem armazenados. Em seguida, em uma variável chamada `profissional`, concatene as variáveis abaixo formando uma *string* que faça sentido com os dados informados e apresente essa variável com o método `document.write()` em algum `arquivo.html` ou utilizando o `console.log()`.

- nome (*string*)
- telefone (*string*)
- se possui convênio médico ou não (*booleano*)
- profissão (*string*)
- salário (*number*)
  
  
```js
    var nome = "Ana";
    var telefone = "(011) 98585-4545";
    var profissao = "vendedora";
    var salario = 1500;
    var profissional = ("Dados do funcionário: Nome: " + nome + "  Telefone: " + telefone +
    "  Cargo: " + profissao + "  Salário: R$ " + salario + " reais.  Possui convênio? " + convenio );
    
    document.write(profissional);
    
    var convenio = false;
      if (convenio){
        document.write("Sim"); 
      }
          
      else {
        document.write("Não possui.");
      }
```
#### 2. Crie uma lógica que armazene dois números inteiros em duas variáveis. Em seguida, troque o valor dessas variáveis e exiba na tela. Por exemplo, uma variável a e outra b, em algum momento a vai valer b, e b vai valer a, mas quando a = b, o valor inicial de apode ser perdido, atenção!

  
```js
var a = 2;
var b = 5;
var aux = a
a=b
b=aux
//se colocar b=a, a resposta será 5, pq eu declarei q a=b, e b=5
// cria se outra variavel para colocar o valor de a 
document.write("a:" +a);
document.write("b:" +b)

```

#### 3. Operações Aritméticas
Realize as operações aritméticas abaixo e exiba os resultados na tela através do console.log():
■ Resolva as operações mentalmente, primeiro, para que possa consolidar melhor os conceitos de variáveis e ordem de precedência.
let inteiro = 7
let decimal = 3.5

- let adicao = inteiro + decimal
- let subtracao = inteiro - decimal
- let potenciacao = (adicao - .5) ** 2
- let expressao1 = inteiro - 4 / 2 / 2
- let expressao2 = (inteiro - 4) / 2
- let expressao3 = 2 + subtracao * 2
- let expressao4 = (2 + subtracao) * 2
- let modulo1 = potenciacao % 2
- let modulo2 = (inteiro - 1) % 2

#### 4. Idade para Votar
No Brasil, uma pessoa é obrigada a votar se tiver idade entre 18 e 70 anos. Acima de 70 anos o voto é opcional, assim como para quem tem 16 ou 17 anos. Quem ainda não completou 16 anos não pode votar. Através de estruturas condicionais, crie um programa que dirá se uma pessoa pode ou não votar, de acordo com a idade que será armazenada em uma variável.

#### 5. Bug no SW - piscina
Uma piscina redonda está sendo construída, e sabe-se que ela tem o raio de 3,5m, e uma altura de 1,6m. O construtor notou um erro no volume de água em litros que o software da empresa está retornando, em torno de 0,06L, e resolveu entrar em contato com a equipe de TI. Construa uma lógica que calcula a quantidade de litros que a piscina suportará e identifique o problema na lógica do software.

#### 6. Estrutura de repetição
Com as estruturas de repetição for e while, faça o que se pede:

- a) Mostre os números de 1 a 50 na tela, dizendo se é par ou ímpar:
- b) Mostre apenas os múltiplos de 3 entre 1 e 100:
- c) Mostre a seguinte sequência (de 100 até 0, pulando de dois em dois):
- d) O jogo do PIM é um jogo em que o Sílvio Santos pedia para os participantes de seu programa contar de 1 até 40 da seguinte forma:
Ou seja, quando o número era múltiplo de 4, o jogador tinha que falar PIM ao invés do número! Crie uma lógica que executa o jogo do PIM corretamente.

#### 7. Fórmulas Matemáticas
A. Crie uma variável para cada figura geométrica(retângulo, círculo, triângulo retângulo), que armazene a fórmula que calcula a sua área.
B. Com as fórmulas armazenadas nessas variáveis, atribua valores em variáveis para as bases, alturas e raio das figuras e calcule
a) a área do retângulo
b) a área do círculo
c) a área do triângulo retângulo
Em seguida exiba os resultados do cálculos das áreas, imprimindo as variáveis através do console.log().

#### 8. Listas
A. Crie uma lista chamada pessoa, coloque valores dentro dela como: nome (string), idade (inteiro), CPF (string), altura (decimal), se é maior de idade ou não (valor booleano true ou false).
B. Crie um programa que recebe uma quantidade máxima de 5 letras e ao final exibe todas elas no console.
Crie uma função chamada recebeLetra para pegar a letra e colocar na lista de letras.
Considerando o exercício anterior, refaça ele criando uma lista que irá armazenar as letras e em seguida mostre no console:
- a) A primeira letra digitada
- b) A quarta letra digitada
- c) A quinta letra digitada
- d) A última letra digitada
- e) O tamanho da lista criada


#### 9. Manipulando valores
Para realizar o que é pedido, crie um arquivo HTML chamado clientes_jessica.html e considere as informações abaixo para resolver o que se pede.
- Jéssica precisa de um programa para calcular e completar informações da sua empresa de forma automática. 
Some as quantidade desses clientes de Jéssica e concatene esse valor numa string semelhante a:
"Nas capitais de BH, SP, BA, MS e PR, Jéssica possui N clientes."
```js
function calculaClientes(bh, sp, ba, ms, pr){
  var clientes = (bh + sp + ba + ms + pr);
  return clientes;
}
var quantidadeClientes = calculaClientes(23,12,11,10,8);
document.write("Nas capitais de BH, SP, BA, MS e PR, Jéssica possui " + quantidadeClientes + "  clientes.");

```
- Calcule a média de faturamento por cliente de cada cidade e obtenha como resultado strings semelhantes a:

"Faturamento médio por cliente:"
"Belo Horizonte: R$ 128"
"São Paulo: R$ 329"
"Salvador: R$ 121"
"Campo Grande: R$ 241"
"Curitiba: R$ 78"

■ Utilize Math.round()!
````js
function calculaFaturamentoMedio(faturamento, cliente){
    var fm = faturamento/cliente;
      return fm;
    }
var fatBeloHorizonte = Math.round(calculaFaturamentoMedio(2950, 23));
var fatSaoPaulo = Math.round(calculaFaturamentoMedio(3950, 12));
var fatSalvador = Math.round(calculaFaturamentoMedio(1329, 11));
var fatCampoGrande = Math.round(calculaFaturamentoMedio(2412, 10));
var fatCuritiba = Math.round(calculaFaturamentoMedio(626, 8));
//var fatCuritiba = (calculaFaturamentoMedio (626, 8).toFixed(2));
                                //outro jeito de arredondar
document.write("O faturamento médio por cliente:");
document.write("<br>Belo Horizonte: R$ " +fatBeloHorizonte); 
document.write("<br>São Paulo: R$ " +fatSaoPaulo);
document.write("<br>Salvador: R$ "+fatSalvador); 
document.write("<br>Campo Grande: R$ "+fatCampoGrande);
document.write("<br>Curitiba: R$ "+fatCuritiba);

````
- Calcule a média de faturamento por cliente, com base em todos os clientes dessas cinco cidades e atribua o valor numa string:
````js
var totalClientes = 23 + 12 + 11 + 10 + 8;
var totalFaturamento = 2950 + 3950 + 1329 + 2412 + 626;
var mediaFaturamentoPorCliente = totalFaturamento / totalClientes;
var resultadoString = "<br>A média de faturamento por cliente nas cinco cidades é de R$ " + mediaFaturamentoPorCliente.toFixed(2);

document.write(resultadoString);
````

- Sabendo que Jéssica oferece frete grátis para seus clientes e possui uma parceria com uma transportadora, considere as seguintes informações sobre os custos com frete que ela possui:
Frete fixo para o estado de São Paulo = R$ 9,00 por produto vendido
Frete para os demais estados do Brasil = R$ 14,00 por produto vendido
O custo de produção dos seus produtos representam 20% do valor faturado (descontando o valor do envio)
Com base nessas informações, ela quer automatizar o cálculo de seu lucro por cidade. Crie as lógicas de cálculos que serão implementadas no programa para preencher a coluna lucro. Utilize console.log() para fazer os testes e lembre-se de utilizar variáveis para armazenar valores.
````js
// Dados sobre os custos de frete e produção
const freteSP = 9.00; // Frete fixo para o estado de São Paulo
const freteOutrosEstados = 14.00; // Frete para os demais estados do Brasil
const custoProducaoPercentual = 0.20; // Custo de produção como percentual do valor faturado

// Dados de faturamento por cidade (já calculados anteriormente)
const faturamentoBeloHorizonte = 2950;
const faturamentoSaoPaulo = 3950;
const faturamentoSalvador = 1329;
const faturamentoCampoGrande = 2412;
const faturamentoCuritiba = 626;

// Função para calcular o lucro
function calcularLucro(faturamento, frete) {
  const custoProducao = faturamento * custoProducaoPercentual;
  const lucro = faturamento - custoProducao - frete;
  return lucro;
}

// Cálculo do lucro para cada cidade
const lucroBeloHorizonte = calcularLucro(faturamentoBeloHorizonte, freteOutrosEstados);
const lucroSaoPaulo = calcularLucro(faturamentoSaoPaulo, freteSP);
const lucroSalvador = calcularLucro(faturamentoSalvador, freteOutrosEstados);
const lucroCampoGrande = calcularLucro(faturamentoCampoGrande, freteOutrosEstados);
const lucroCuritiba = calcularLucro(faturamentoCuritiba, freteOutrosEstados);

// Exibição dos resultados
document.write( "<br>Lucro por cidade:");
document.write(`<br>Belo Horizonte: R$ ${lucroBeloHorizonte.toFixed(2)}`);
document.write(`<br>São Paulo: R$ ${lucroSaoPaulo.toFixed(2)}`);
document.write(`<br>Salvador: R$ ${lucroSalvador.toFixed(2)}`);
document.write(`<br>Campo Grande: R$ ${lucroCampoGrande.toFixed(2)}`);
document.write(`<br>Curitiba: R$ ${lucroCuritiba.toFixed(2)}`);
````




