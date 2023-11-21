## Instrução de como rodar o codigo baixo:

•	Entre em um site de compilador online pode ser o: https://codepen.io/ 

•	Cole o codigo completo no compilador

•	Execute o codigo 

•	Escolha a opção 1 do menu 

•	Escolha um numero que deseja ver a somatoria 


## A função somatoria implementada em JavaScript, podendo ser rodada em qualquer ambiente que tenha o JS ou em algum compilador online
Aqui é o menu da função, aonde o usuario escolhe qual parte da codigo deseja de seguir 

     do{ //  permite que o usuário faça escolhas repetidas até optar por sair
    let opcao = parseInt(prompt("\nA seguir vamos implementar uma função que receba um número inteiro positivo e retorne o somatório de todos os valores inteiros divisíveis por 3 ou 5 que sejam inferiores ao número passado. \n \nA Seguir digite o numero da opção abaixo: \n \n" +
     "[1] = Inserir o numero para para implemantar a função \n" +
     "[2] = Sair da função \n"));
     switch(opcao){ // aqui implementei um Switch para ter as opções abaixo de Inserir um numero ou de Sair do programa 
        case 1:
           somarMultiplos();           
            break;
        case 2:
            alert("Encerrando o Programa");
            break;
        default:
                alert("Opção inválida. Escolha uma opção de 1 a 2.");
     }}while(opcao !== 2);

# A seguir a função  faz que o codigo verifica se o numero é dividido por 3 ou 5 

A função somarMultiplos recebe um número do usuário, verifica se é um inteiro positivo e, em seguida, calcula o somatório dos múltiplos de 3 ou 5 menores que o número fornecido.

  
    function somarMultiplos(){
    let num; //  
    let somatorio=0;
    let resultado 
    num = parseInt(prompt("Digite o numero que deseja ver a somatorio"));
    for( let i = 1 ;i < num; i++){ // Faz um for para ir contanto ate o numero digitado e quando chegar no numero digitado ele para 
        if(i% 3 === 0 || i % 5 === 0){ // Verifica se o numero é dividido por ambos 3 e 5 
            somatorio += i; // apos passar por toda a contagem ele vai somando o valor 
        }
    }
    resultado = somatorio;
    alert("O somatório dos múltiplos de 3 ou 5 inferiores é " + num + " é: " + resultado);
    }

# A seguir a função completa 
    let opcao;
    function somarMultiplos(){
    let num; //  
    let somatorio=0;
    let resultado 
    num = parseInt(prompt("\nDigite o numero que deseja ver a somatorio"));
    for( let i = 1 ;i < num; i++){ // Faz um for para ir contanto ate o numero digitado e quando chegar no numero digitado ele para 
        if(i% 3 === 0 || i % 5 === 0){ // Verifica se o numero é dividido por ambos 3 e 5 
            somatorio += i; // apos passar por toda a contagem ele vai somando o valor 
        }
    }
    resultado = somatorio;
    alert("O somatório dos múltiplos de 3 ou 5 inferiores é " + num + " é: " + resultado + "\n");
    }
    do{
    opcao = parseInt(prompt("A seguir vamos implementar uma função que receba um número inteiro positivo e retorne o somatório de todos os valores inteiros divisíveis por 3 ou 5 que sejam inferiores ao número passado. \n \nA Seguir digite o numero da opção abaixo: \n \n" +
     "[1] = Inserir o numero para para implemantar a função \n" +
     "[2] = Sair da função \n"));
     switch(opcao){ // aqui implementei um Switch para ter as opções abaixo de Inserir um numero ou de Sair do programa 
        case 1:
           somarMultiplos();           
            break;
        case 2:
            alert("Encerrando o Programa");
            break;
        default:
                alert("Opção inválida. Escolha uma opção de 1 a 2.");
     }}while(opcao !== 2);


  
  
