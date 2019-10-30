# Etiquetas


# Linguagens

<strong>DPL – Datamax Programming Language</strong> – Linguagem de programação desenvolvida para modelos da impressora Datamax

<strong>ZPL – Zebra Programming Language</strong> – Linguagem de programação desenvolvida para modelos de impressoras Zebras Technologies

<strong>EPL – Eltron Programming Language</strong> – Linguagem de programação desenvolvida para impressoras Eltron, antigo fabricante e hoje pertence a Zebra Technologies;

<strong>IPL – Intermec Programming Language</strong> – Linguagem de programação desenvolvida para impressora Intermec

<strong>PPLA – Printer Programming Language A</strong> – Linguagem de programação que emula o conjunto de comando DPL ( Datamax Programming Language ). Simulam a mesma linguagem e permitem que softwares que foram desenvolvidos para o envio de comando DPL, sejam compatíveis mesmo não utilizando impressora Datamax.

<strong>PPLB – Printer Programming Language B</strong> – Linguagem de programação que emula o conjunto de comando EPL ( Eltron Programming Language ) .


# Exemplo

<code>
I8,A,001


Q224,024
q831
rN
S4
<strong>D</strong>7
ZT
JF
OD
R16,0
f100
N
A784,200,2,4,1,1,N,"<strong>[DESCRICAO]</strong>"
A433,80,2,4,1,1,N,"<strong>[FANTASIA]</strong>"
A783,49,2,4,1,1,N,"<strong>[CODIGO]</strong>"
B762,165,2,E30,2,4,94,B,"<strong>[CODBARRAS]</strong>"
A392,147,2,5,1,1,N,"<strong>[VALOR]</strong>"
<strong>P</strong>1

</code>

As informações em <strong>Negrito</strong>, são informações que o software precisará alterar 
para realizar a impressao das etiquetas.

