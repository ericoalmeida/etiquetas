# Etiquetas


# Linguagens

<strong>DPL – Datamax Programming Language</strong> – Linguagem de programação desenvolvida para modelos da impressora Datamax

<strong>ZPL – Zebra Programming Language</strong> – Linguagem de programação desenvolvida para modelos de impressoras Zebras Technologies

<strong>EPL – Eltron Programming Language</strong> – Linguagem de programação desenvolvida para impressoras Eltron, antigo fabricante e hoje pertence a Zebra Technologies;

<strong>IPL – Intermec Programming Language</strong> – Linguagem de programação desenvolvida para impressora Intermec

<strong>PPLA – Printer Programming Language A</strong> – Linguagem de programação que emula o conjunto de comando DPL ( Datamax Programming Language ). Simulam a mesma linguagem e permitem que softwares que foram desenvolvidos para o envio de comando DPL, sejam compatíveis mesmo não utilizando impressora Datamax.

<strong>PPLB – Printer Programming Language B</strong> – Linguagem de programação que emula o conjunto de comando EPL ( Eltron Programming Language ) .


# Exemplo

> Etiqueta utilizando a linguagem PPLB.

```
I8,A,001


Q224,024
q831
rN
S4
D7
ZT
JF
OD
R16,0
f100
N
A784,200,2,4,1,1,N,"[DESCRICAO]"
A433,80,2,4,1,1,N,"[FANTASIA]"
A783,49,2,4,1,1,N,"[CODIGO]"
B762,165,2,E30,2,4,94,B,"[CODBARRAS]"
A392,147,2,5,1,1,N,"[VALOR]"
P1

```

# Parâmetros

O parâmetro <strong>"D"</strong> representado abaixo: e o valor da temperatura da cabeça de impressão.
> Recebe um valor entre 0 e 15.
```
D7
```

Os parâmetros entre <strong>" "</strong> representado abaixo: serão substituídos pelos valores correspondentes
de cada produto. <br />
>Software ERP deve ler as variáveis e substituir pela informação correpondente do produto.
```
A784,200,2,4,1,1,N,"[DESCRICAO]"
```

O parâmetro <strong>"P"</strong> representado abaixo: e o numero de linhas a ser impressa. <br />
<i> Se a etiqueta for de 3 colunas, ou seja, 3 etiquetas por linha. nesse parametro estiver configurado com o valor 2. será impresso 6 etiquetas. </i>
```
P1
```