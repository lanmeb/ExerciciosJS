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
