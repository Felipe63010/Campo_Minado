# Campo Minado (Python)

Esse é um código simples que simula o jogo Campo Minado, o qual é jogado no terminal. O jogador escolhe o tamanho do mapa e o número de minas que ele irá enfrentar, o player deve encontrar e marcar todas as minas sem abrir nehuma delas. 

## Funcionalidades

* O tamanho do mapa é definido pelo usuário:
    * mínimo: 1 linha × 1 coluna
    * máximo: 10 linhas × 10 colunas
* O usuário pode decidir a dificuldade do jogo, uma vez que ele que escolhe o número de minas, mas as posições delas são aleatórias.
* O usuário pode marcar posições com a letra M. 
* O usuário pode abrir uma posição, assim, tornando possível descobrir quantas bombas existem nas 8 posições em volta da qual ele abriu (na posição aberta fica o número de bombas que se encontra nos arredores).


## Formas de Vencer e Perder

* O jogador deve marcar todas as posições que contém mina com a letra M.
* O jogador não deve abrir uma posição que contém mina, uma vez que caso isso aconteça ele irá perder.

## Como Executar
* Para jogar, você precisa ter o Python 3 instalado em sua máquina, aí é necessario baixar o arquivo Campo_Minado.py,abrir o terminal e navegar ate o diretorio do arquivo e tem que executar o script com /bin/python3 /home/felipe/Documentos/Campo_Minado/Campo_Minado.py

### Como jogar

* Quando o programa for executado solicitará:
    * O número de linhas do Mapa
    * O número de colunas do Mapa
    * O número de minas do Mapa 

* Em cada rodada, o usuário pode escolher duas opções:
    * Marcar posições que o jogador acredita que tem bomba com a letra M.
    * Abrir posição para revelar as 8 posiçoes que fazem fronteira com a cordenada escolhida.

## Interface
* No início do código os inputs do tamanho do mapa e do número de minas serão mostrados ao usuário com algumas restrições explícitas para que o usuário não cometa erros e caso cometa o usuário volta do início, sendo necessário colocar os inputs novamente.
* Após essa inserção inicial o mapa será mostrado.
* Seguindo o código aparecerá um menu, no qual o usuário poderá escolher entre abrir uma posição, marcar uma posição e desistir (nas duas primeiras uma cordenada é pedida).
* Ao final do jogo se o jogador venceu (marcou todas as minas de forma correta) aparecerá uma mensagem indicando que ele venceu, caso o usuário seja derrotado (tente abrir uma posição, na qual há bomba) uma mensagem indicando que ele perdeu aparecerá e caso ele desista uma mensagem de desistência será exibida. Em todas essas ocasiões o programa é encerrado.

## Descrição Final

* Este projeto utiliza apenas bibliotecas padrão do Python, sem necessidade de instalação de pacotes externos.

*  Random (para a geração aleatória das minas)
* Copy (para copiar uma matriz em outra)