# Help-SSL

Antes de Falar de SSL precisamos abordar o HTTPS:

## HTTP 
###### Hypertext Transfer Protocol / Protocolo de Transferência de Hipertexto
HTTP é um protocolo de transferência que possibilita que as pessoas que inserem a URL de um site na Web possam ver os conteúdos e dados que nele existem. 

Qualquer servidor que você escolha para hospedar o site da sua empresa tem um <ins>programa projetado para receber solicitações HTTP<ins>. 
Portanto, o navegador que você usa é um cliente HTTP que envia solicitações constantemente ao seu servidor.

###### Como acontece todo o processo:
1. Se a URL pertencer a um domínio próprio, o navegador primeiro se conecta a um servidor e recuperará o endereço IP correspondente ao servidor;
2. O navegador se conecta ao servidor e envia uma solicitação HTTP para a página da web desejada (que, neste exemplo, é o seu site);
3. O servidor recebe a solicitação e verifica a página desejada. Se a página existir, o servidor a mostrará. Se o servidor não conseguir encontrar a página solicitada, ele enviará uma mensagem de erro HTTP 404, ou seja, página não encontrada;
4. O navegador, então, recebe a página de volta e a conexão é fechada;
5. Caso a página exista (e é isso que se espera), o navegador a analisa e procura outros elementos necessários para concluir a sua exibição, o que inclui seus textos, imagens e afins;
6. Para cada um desses elementos, o navegador faz conexões adicionais e solicitações HTTP para o servidor para cada elemento;
7. Quando o navegador terminar de carregar todos os elementos, a página será carregada na janela do navegador.


## HTTPS
###### Hypertext Transfer Protocol Secury / Protocolo de Transferência de Hipertexto Seguro
O HTTPS é uma extensão do HTTP. O “S” vem da palavra “secure” (“segurança” em inglês) e costuma ser oferecido pelo **certificado SSL**, 
oferecidos pela maioria dos servidores. Ele oferece uma **conexão criptografada entre o servidor e o navegador**, de maneira que o usuário possa inserir informações 
com mais segurança.


## SSL
##### Secure Sockets Layer / Camada Segura
O SSL (Secure Sockets Layer) usa um sistema de criptografia que utiliza duas chaves para criptografar os dados, uma chave pública conhecida por todos e uma chave privada conhecida apenas pelo destinatário/servidor da aplicação.

É o mesmo conceito de criptografia assimétrica do algoritmo RS256 utilizado no _Jason Web Token_ (JWT).

Uma conexão SSL/TLS em funcionamento garante que os dados sejam enviados e recebidos do servidor correto, em vez de um “homem do meio” mal-intencionado. Isto é, ajuda a impedir que os agentes maliciosos falsifiquem um site.

Outro benefício é a **integridade dos dados**. As conexões SSL/TLS garantem que não haja perda ou alteração de dados durante o transporte, incluindo um código de autenticação de mensagem (MAC). Isso garante que os dados enviados sejam recebidos sem alterações ou alterações maliciosas.


