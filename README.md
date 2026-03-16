## Introducao-Computacao-Hardware
 Atividade de Introdução à Computação

## Feito em colaboração com Sara Rebeca do Rosário Soares

# Investigação de Hardware: Supercomputador Cray-1

##### Descrição

O Cray-1 foi um Supercomputador desenvolvido e manufaturado pela Cray Research, uma empresa produtora de supercomputadores sediada em Minnesota, EUA. O seu primeiro modelo foi criado em 1976, e foi considerado o computador mais rápido da época, entre 1976 e 1982, sendo cerca de 10 vezes mais rápido do que os computadores concorrentes da época. Mas custava até $10M ( hoje em dia, R$53.306.010). e consumia 115 KW de energia, o suficiente para alimentar 10 casas.

![Cray-1](http://images.computerhistory.org/revonline/images/x1553.98ap-03-01.jpg?w=600)

### Análise Técnica

Para Analise técnica, o Cray-1 será comparado com um processador moderno i9-9900K

#### Processamento - Cray-1

##### ULA

Possuia 12 unidades funcionais independentes, divididas em 4 grupos (Adress, Escalar, Vetorial, Flutuante),  essas sendo totalmente segmentadas. 

Suportava operações de adição, subtração, multiplicação, divisão e aproximação de recíproco para números flutuantes, e para inteiros, suportava adição, subtração e multiplicação.

Também tinha incluido operações lógicas/Booleanas, de OR, AND e XOR.

##### Unidade de Controle

Todas as instruções eram executadas a partir de quatro buffers de instrução, cada um com 64 registradores  de 16 bits, e cada buffer possuindo um registrador de endereço base para determinar se a instrução atual residia nele.

As unidades funcionais recebiam operandos  dos registradores e entregavam o resultado a um registrador ao concluir a operação. E operavam em modo de três endereços

Todas as unidades funcionais executavam seus algoritmos em tempo fixo, e múltiplas unidades funcionais podiam operar simultaneamente, sendo independentes entre si.

#### Processamento - i9-9900K

##### ULA

O i9-9900K possui um back-end superescalar da Skylake (codinome da Intel para a sua sexta geração de microprocessadores) com 8 portas de execução, cada uma com  até 20 unidades funcionais especializadas. Dessas portas, 4 são de execução inteira, 2 são AGU de propósito geral, e uma porta é exclusiva de store.

O processador pode fazer uma quantidade de operações muito maior  do que o Cray-1, tanto para pontos flutuantes e vetoriais, quanto para inteiros e operações de memórias.

##### Unidade de Controle

A UC do i9-9900K é distribuida pelo front-end e back-end, tendo 14 estágios.
No Front-End, ocorre a busca e decodificação, onde uma instrução é buscada, depois decodificada, depois executada e somente então retirada. Esse processo é sobreposto entre instruções adjacentes. Ou seja, enquanto uma está sendo retirada, a seguinte já está sendo executada, a próxima sendo decodificada, e a outra sendo buscada.

No Back-End, é onde há a execução fora  de ordem, onde as micro-operações passam por um Buffer de Reorganização (ROB/Reorder Buffer), onde ocorrem alocação de registradores, renomeamento e o retiring. O ROB do Skylake tem 224 entradas.

#### Armazenamento - Cray-1

Possuía cinco conjuntos de registradores, sendo 3 primários (Address, Escalar e Vetorial), que eram acessíveis diretamente pelas unidades funcionais, e 2 intermediários (Address intermediário e Escalar intermediário). Os registradores intermediários de endereço e escalares, ambos com 64 bits cada, podiam ser preenchidos por transferências em bloco a partir da memória.

Sua memória era construída com chips LSI de 1024 bits, e até 1.048.576 palavras de 72 bits, sendo 64 bits de dados somados a 8 bits de verificação. No total, equivale a uma memória RAM de cerca de 8 MegaBytes e 152 registradores no total.

#### Armazenamento - i9-9900K

Possui 64KB de cache L1 por núcleo, 256 KB de cache L2 por núcleo e 16 MB de cache L3 compartilhado. Seu chip suporta até 128 GiB de memória DDR4-2666 em canal duplo.

#### Interface - Cray-1

A sua entrada e saída era feita através de 24 canais de Input/Output. 12 de entrada e 12 de saída, qualquer um desses canais podendo estar ativos ao mesmo tempo. A entrada e saída compartilhavam o acesso à memória via uma única porta.

O Cray-1 podia ser conectado a sistemas front-end por meio de controladores especiais da empresa Cray Research, que compensavam diferenças em larguras de canal, tamanho de palavra e máquina. 
Também possuia  periféricos de saída como uma impressora e o plotter, que eram conectados ao subsistema de armazenamento em massa.

O sistema também suportava equipamentos externos fornecidos pelo usuário, como unidades de fita magnética, que eram usadas para staging de conjuntos de dados entre o armazenamento em massa do sistema e os dispositivos periféricos.

#### Interface - i9-9900K

O processador suporta overclocking, 16 lanes PCIe 3.0 (direto no processador) e USB 3.1 Gen2. O chip incorpora a GPU integrada Intel UHD Graphics 630, operando a 350 MHz com frequência burst de 1,2 GHz

### Referências

Wikipedia. Cray-1. https://en.wikipedia.org/wiki/Cray-1

Computer History Museum. The Cray-1 Supercomputer. https://www.computerhistory.org/revolution/supercomputers/10/7

Cray Research, inc. (CRI), The Cray-1 Computer System. 1977. E.U.A. https://www.computerhistory.org/brochures/doc-43729572b49ef/

Intel®. Intel® 64 and IA-32 Architectures Software Developer Manuals. https://www.intel.com/content/www/us/en/developer/articles/technical/intel-sdm.html

Wikipedia. List of Intel CPU microarchitectures. https://en.wikipedia.org/wiki/List_of_Intel_CPU_microarchitectures

Wikipedia. Skylake (microarchitecture). https://en.wikipedia.org/wiki/Skylake_(microarchitecture)

desklib. Analysis of Intel Core i9-9900K Processor Architecture and Features. https://desklib.com/study-documents/intel-core-i9-9900k-architecture-1/

DELGADO, J.; RIBEIRO, C. Arquitetura de Computadores. São Paulo: Grupo GEN, 2017. MINHA BIBLIOTECA (CeUB
