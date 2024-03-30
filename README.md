## Exercicios em Java Script

#### 1. Crie 5 variáveis e atribua valores, respeitando os tipos de dados a serem armazenados. Em seguida, em uma variável chamada `profissional`, concatene as variáveis abaixo formando uma *string* que faça sentido com os dados informados e apresente essa variável com o método `document.write()` em algum `arquivo.html` ou utilizando o `console.log()`.

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

#### 3. Realize as operações aritméticas abaixo e exiba os resultados na tela através do console.log():
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

#### 4. No Brasil, uma pessoa é obrigada a votar se tiver idade entre 18 e 70 anos. Acima de 70 anos o voto é opcional, assim como para quem tem 16 ou 17 anos. Quem ainda não completou 16 anos não pode votar. Através de estruturas condicionais, crie um programa que dirá se uma pessoa pode ou não votar, de acordo com a idade que será armazenada em uma variável.

#### 5. Uma piscina redonda está sendo construída, e sabe-se que ela tem o raio de 3,5m, e uma altura de 1,6m. O construtor notou um erro no volume de água em litros que o software da empresa está retornando, em torno de 0,06L, e resolveu entrar em contato com a equipe de TI. Construa uma lógica que calcula a quantidade de litros que a piscina suportará e identifique o problema na lógica do software.

#### 6.
1. Com as estruturas de repetição for e while, faça o que se pede:

- a) Mostre os números de 1 a 50 na tela, dizendo se é par ou ímpar:
- b) Mostre apenas os múltiplos de 3 entre 1 e 100:
- c) Mostre a seguinte sequência (de 100 até 0, pulando de dois em dois):
- 
2. O jogo do PIM é um jogo em que o Sílvio Santos pedia para os participantes de seu programa contar de 1 até 40 da seguinte forma:
Ou seja, quando o número era múltiplo de 4, o jogador tinha que falar PIM ao invés do número! Crie uma lógica que executa o jogo do PIM corretamente.

#### 7.
Para realizar o que é pedido, crie um arquivo HTML chamado clientes_jessica.html e considere as informações abaixo para resolver o que se pede.
- Jéssica precisa de um programa para calcular e completar informações da sua empresa de forma automática. A tabela abaixo mostra alguns dados das 5 primeiras cidades onde ela mais possui clientes ativos:

- 1. Some as quantidade desses clientes de Jéssica e concatene esse valor numa string semelhante a:
"Nas capitais de BH, SP, BA, MS e PR, Jéssica possui N clientes."

