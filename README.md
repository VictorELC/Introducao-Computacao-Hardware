## Introducao-Computacao-Hardware
 Atividade de Introdução à Computação

# Investigação de Hardware: Supercomputador Cray-1

##### Descrição
O Cray-1 foi um Supercomputador desenvolvido e manufaturado pela Cray Research, uma empresa produtora de supercomputadores com sede em Seattle, EUA. O seu primeiro modelo foi criado em 1976, e foi considerado o computador mais rápido da época, entre 1976 e 1982, sendo cerca de 10 vezes mais rápido do que os computadores concorrentes da época. Mas custava até $10M ( hoje em dia, R$53.306.010). e consumia 115 KW de energia, o suficiente para alimentar 10 casas.

![Cray-1](http://images.computerhistory.org/revonline/images/x1553.98ap-03-01.jpg?w=600)

### Análise Técnica

#### Processamento - Cray-1

##### ULA

Possuia 12 unidades funcionais independentes, divididas em 4 grupos (Adress, Escalar, Vetorial, Flutuante),  essas sendo totalmente segmentadas. 

Suportava operações de adição, subtração, multiplicação, divisão e aproximação de recíproco para números flutuantes, e para inteiros, suportava adição, subtração e multiplicação.

Também tinha incluido operações lógicas/Booleanas, de OR, AND e XOR.

##### Unidade de Controle

Todas as instruções eram executadas a partir de quatro buffers de instrução, cada um com 64 registradores  de 16 bits, e cada buffer possuindo um registrador de endereço base para determinar se a instrução atual residia nele.

As unidades funcionais recebiam operandos  dos registradores e entregavam o resultado a um registrador ao concluir a operação. E operavam em modo de três endereços

Todas as unidades funcionais executavam seus algoritmos em tempo fixo, e múltiplas unidades funcionais podiam operar simultaneamente, sendo independentes entre si.

#### Armazenamento - Cray-1

Possuía cinco conjuntos de registradores, sendo 3 primários (Adress, Escalar e Vetorial), que eram acessíveis diretamente pelas unidades funcionais, e 2 intermediários (Adress intermediário e Escalar intermediário). Os registradores intermediários de endereço e escalares, ambos com 64 bits cada, podiam ser preenchidos por transferências em bloco a partir da memória.

Sua memória era construída com chips LSI de 1024 bits, e até 1.048.576 palavras de 72 bits, sendo 64 bits de dados somados a 8 bits de verificação. No total, equivale a uma memória RAM de cerca de 8 MegaBytes e 152 registradores no total.

#### Interface - Cray-1

A sua entrada e saída era feita através ded 24 canais de Input/Output. 12 de entrada e 12 de saída, qualquer um desses canais ´podendo estar ativos ao mesmo tempo. A entrada e saída compartilhavam o acesso à memória via uma única porta.

O Cray-1 podia ser conectado a sistemas front-end por meio de controladores especiais da empresa Cray Research, que compensavam diferenças em larguras de canal, tamanho de palavra e máquina. 
Também possuia  periféricos de saída como uma impressora e o plotter, que eram conectados ao subsistema de armazenamento em massa.

O sistema também suportava equipamentos externos fornecidos pelo usuário, como unidades de fita magnética, que eram usadas para staging de conjuntos de dados entre o armazenamento em massa do sistema e os dispositivos periféricos.

### Referências

Página da Wikipédia do Cray-1. https://en.wikipedia.org/wiki/Cray-1

Museu da História da Computação. The Cray-1 Supercomputer. https://www.computerhistory.org/revolution/supercomputers/10/7

Cray Research, inc. (CRI), The Cray-1 Computer System. 1977. E.U.A. https://www.computerhistory.org/brochures/doc-43729572b49ef/
