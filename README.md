Jogo do Número Secreto - README

Este é um simples jogo de adivinhação desenvolvido em JavaScript, no qual o objetivo é descobrir um número secreto gerado aleatoriamente dentro de um intervalo de 1 a 10. O jogo fornece dicas para ajudar o jogador a acertar e mantém um contador de tentativas. 
Abaixo, você encontrará uma explicação detalhada sobre o funcionamento e as principais funcionalidades do código.

---

Como o jogo funciona:

1. Objetivo: O jogador precisa adivinhar o número secreto, que é gerado aleatoriamente entre 1 e 10, sem repetir números sorteados anteriormente até que todos os números sejam usados.

2. Interatividade:

O jogador insere um número em um campo de texto.
O jogo avalia se o número corresponde ao número secreto.
Caso o palpite esteja errado, o jogo dá uma dica informando se o número secreto é maior ou menor.
O número de tentativas é contabilizado até que o jogador acerte.

3. Reinício: Após acertar, o jogador pode reiniciar o jogo, e um novo número secreto será gerado.




---

Principais componentes do código:

1. Variáveis principais

listaDeNumerosSorteados: Lista que mantém os números já sorteados para evitar repetições.

numeroLimite: O limite superior do intervalo de números (neste caso, 10).

numeroSecreto: O número gerado aleatoriamente que o jogador precisa adivinhar.

tentativas: Contador de tentativas feitas pelo jogador.

---

2. Funções principais

1. gerarNumeroAleatorio()

Gera um número aleatório entre 1 e o numeroLimite.
Garante que o número gerado ainda não foi utilizado, adicionando-o à lista listaDeNumerosSorteados.
Reinicia a lista de números sorteados se todos os números já foram utilizados.


2. exibirTextoNaTela(tag, texto)

Atualiza o texto exibido em elementos HTML, como títulos (h1) e parágrafos (p).
Utiliza a biblioteca responsiveVoice para converter o texto em áudio, fornecendo feedback sonoro ao jogador.


3. verificarChute()

Obtém o número inserido pelo jogador.
Compara o palpite com o número secreto:
Se o palpite estiver correto, exibe uma mensagem de vitória.
Se o palpite estiver errado, fornece uma dica indicando se o número secreto é maior ou menor.
Incrementa o contador de tentativas.


4. limparCampo()

Limpa o campo de entrada para que o jogador insira um novo número.


5. reiniciarJogo()

Reinicia o jogo gerando um novo número secreto.
Reseta o contador de tentativas.
Desativa o botão de reinício até que o jogador acerte novamente.


6. exibirMensagemInicial()
   
Exibe a mensagem inicial do jogo, orientando o jogador sobre como jogar.

---

Como jogar:

1. Abra o jogo em um navegador compatível com JavaScript e a biblioteca responsiveVoice.
2. Leia ou ouça as instruções iniciais.
3. Insira um número no campo de entrada e clique em um botão (ou pressione Enter) para enviar o palpite.
4. Receba dicas sobre o número secreto.
5. Continue tentando até acertar. O jogo exibirá a mensagem de vitória com o número de tentativas.
6. Clique no botão "Reiniciar" para jogar novamente.
