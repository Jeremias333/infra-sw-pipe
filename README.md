# [INFRAESTRUTURA DE SOFTWARE] Processo pai escreve, processo filho lê.

> Como compilar o programa:<br>
Após clonar o repositório utilize o comando abaixo para criar o build<br>
`make build`

<br>

> Como rodar o programa: <br>
`make run`

<br>

> Como limpar a compilação gerada: <br>
`make clean`

<br>

> Lógica utilizada: <br>

#### Para uma melhor compreensão, utilizei como base o código de processo zumbi da última aula <br> uni o código visto em sala/disponibilizado no classroom e dividi os processos antes da execução do fork(divisão entre pai e filho). Nisso utilizamos, a parte da escrita e o compartilhamento de variáveis, antes do fork, e deixando apenas quando o PID == 0 ou seja o filho, para executar a leitura.

<br>

obs: Ocorreu uma anomalia no código, de alguma forma que não deu tempo de entender o output é esse: <br>

Writing Message 0 is Maria <br>
Writing Message 1 is Joao andou a noite <br>
Reading Message 0 is Maria <br>
Reading Message 1 is Maria <br>

