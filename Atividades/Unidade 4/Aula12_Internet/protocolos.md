# Protocolos

### TCP/IP

É o protocolo fundamental da internet, sendo o conjunto entre Internet Protocol (IP), que determina de onde vem e para onde vai cada dado, e Transmission Control Protocol (TCP), que divide os dados em pequenos pacotes, envia, e garante que todos cheguem ao seu devido destino na ordem certa.

Quando você baixa um arquivo, por exemplo, o IP encontra os dados a serem enviados, e o TCP Garante que todos os pedaços dos dados cheguem completos.

### HTTP e HTTPS

HTTP, ou HyperText Transfer Protocol, é o protocolo que define a forma de troca de informações entre servidores web. O HTTPS é o mesmo, mas com uma camada de segurança que criptografa os dados trafegados, permitindo que mesmo com a interceptação  da comunicação, a leitura não seja permitida.

Um exemplo seria qualquer site que precise de algum tipo de login, que começará em HTTPS. Um site apenas em HTTP não precisa de login, e esses dados trafegam em texto puro.

### DNS

DNS, ou Domain Name System, é o sistema que traduz os nomes de domínio legíveis em endereços IP, que são legíveis para máquinas. 
Por exemplo: Ao digitar qualquer site, seu dispositivo consulta um servidor DNS, que traduz o nome legível para o IP correspondente, e apenas após isso, o navegador consegue se conectar ao servidor correto.

### FTP

FTP, ou File Transfer Protocol, é um protocolo criado especificamente para transferência de arquivos entre computadores em uma rede. Funciona com dois canais separados, um para comandos, e outra para a transferência dos dados em si.
Exemplo: desenvolvedores web costumam usar o FTP para enviar arquivos de um site do seu computador para o servidor de hospedagem. 
