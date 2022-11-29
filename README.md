# ⚪🔴🔵🟢 mastermind🕹️
Projeto para a matéria PCS3115 - Sistemas Digitais I - utilizando circuitos combinacionais e sequenciais para reprodução do jogo "mastermind" ou  "senha".

![foto do jogo mastermind](https://m.media-amazon.com/images/I/81Dl8jsSJ4L._AC_SL1500_.jpg)

Bem-vindos ao nosso repositório :)! Nesse README, explicaremos como testar e executar nosso projeto, utilizando os arquivos em verilog e o testbench incluidos aqui. Além disso, também instruiremos a utilização do software "Logisim", que permite simular circuitos digitais, no qual simulamos o nosso projeto, possibilitanto a interação com o jogo e trazendo um pouco de diversão^^!

## Testbench
Para executá-lo, siga os seguintes passos:

1. Ter o VSCode, o Questa e o Quartus instalado, para isso, você pode seguir o tutorial fornecido pelos professores da disciplina no moodle, aula 7. 
2. Deixar a pasta que contém os arquivos em verilog e o testbench no mesmo ambiente em que estão o Questa e Quartus instalados.
3. Agora, para poder compilar os arquivos, escreva, em ordem, os seguintes comandos no terminal do VSCode:
````
vlog nome_do_codigo.v
````
```
vlog nome_do_codigo_tb.v
```
```
vsim -c nome_da_pasta_com_os_arquivos.nome_do_codigo_tb
```
4. Após compilar, você deve digitar o seguinte comando no terminal:
```
run 1600ns
```
Sendo "1600ns" a unidade de tempo para o testbench rodar. Para os nossos arquivos, recomendamos 800ns ou 1600ns.

Com tudo isso feito, você verá no terminal os valores das entradas e saídas dos nossos módulos.

Para melhor entendimento, segue um exemplo dos comandos para o teste do nosso _encoder_, que está dentro da pasta _work_.

````
vlog encod4x2.v
````
```
vlog encod4x2_tb.v
```
```
vsim -c work.encod4x2_tb
```

## Logisim
Para poder jogar o "senha", você precisará seguir os seguintes passos:
1. Baixar o software utilizado através [desse](https://sourceforge.net/projects/logisimevolution/) link.
2. Assim que baixado, basta abrir o arquivo (que foi enviado em uma pasta.zip juntamente com o relatório do projeto) com o Logisim e acessar o circuito de nome "Hipocomp". Assim você poderá se divertir gravando uma senha e tentando acertá-la!!
