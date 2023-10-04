# HTTP Entendendo a WEB por baixo dos panos

## Aula 01 Conhecendo o protocolo HTTP - video 1
**HTTP, Hyper Text Transfer Protocol**
Em tradução livre, o significado em português seria "Protocolo de Transferência de Hipertexto" (hipertexto é um texto que contém links para outros textos, como por exemplo o HTML que permite o uso de links para outras páginas).
Nesta aula, o instrutor introduziu o conceito de HTTP (Hypertext Transfer Protocol) e explorou como ele é utilizado no projeto AluraBooks, tanto no Back-End quanto no Front-End. O HTTP é um protocolo de comunicação usado para transferir dados na web e é amplamente utilizado em todos os sites do mundo.
No Back-End do AluraBooks, o HTTP é utilizado para receber e processar as requisições feitas pelo cliente. O instrutor demonstrou como iniciar o projeto no Terminal e observar as informações relacionadas ao HTTP, como a URL da requisição, o método utilizado e o código de status. Além disso, é possível visualizar o payload da requisição, que corresponde às informações preenchidas pelo usuário na tela de cadastro.
No Front-End do AluraBooks, o HTTP é utilizado para enviar as requisições para o Back-End. O instrutor mostrou como iniciar o Front-End e utilizar a aba "Rede" no console do navegador para visualizar as requisições HTTP. Ao interagir com a página, como clicar no botão de cadastro, é gerada uma requisição HTTP que pode ser observada na aba "Rede". O instrutor destacou a importância de entender que o HTTP é uma interação entre o cliente (Front-End) e o servidor (Back-End).
O vídeo encerrou com uma breve explicação sobre o significado da sigla HTTP e a sua função de transferir dados na web. O instrutor mencionou que a arquitetura HTTP é composta por um cliente e um servidor, mas deixou para abordar esse assunto em vídeos futuros.


## Aula 01 Conhecendo o protocolo HTTP - video 2
Nesta aula, foi abordada a arquitetura do protocolo HTTP, que é responsável pela comunicação entre o Front-End e o Back-End de um projeto. Foram explicadas as camadas da internet, desde a física até a de aplicação, onde o HTTP está presente. Também foi mencionado que o HTTP roda sobre o TCP, garantindo o envio de mensagens com sucesso. No contexto do projeto AluraBooks, o HTTP é utilizado em um ambiente de desenvolvimento com todas as entidades em um único computador. O próximo vídeo abordará endereços e URLs.

## Aula 01 Conclusão - Nessa aula, você aprendeu a:
Configurar o AluraBooks, o projeto que utilizaremos ao longo do curso;
Contextualizar o HTTP nas camadas da Internet;
Caracterizar o que é o HTTP, e quais os seus principais componentes;
Identificar a arquitetura das comunicações utilizando HTTP.


## Aula 02 Entendendo URLs - video 1
Nesta aula, o instrutor discute sobre a estrutura de um projeto em termos de arquitetura, como clientes e servidor, trocando mensagens HTTP. Ele aborda as diferentes páginas que podem ser acessadas usando HTTP e como nos referimos a cada página específica. O instrutor também menciona a necessidade de nomear as páginas de forma que qualquer pessoa possa entendê-las e colocá-las no navegador para buscá-las. Em seguida, ele introduz o conceito de URL (Uniform Resource Locator), que é um mecanismo padronizado para nomear páginas. Ele explica as diferentes partes da URL e como ela permite acessar recursos em diferentes aplicações web, dispositivos móveis, servidores e desktops. O conhecimento sobre URLs pode ser usado para entender melhor como funcionam os domínios e como estruturar e criar novas páginas no sistema web em desenvolvimento.

**URI, URL ou URN?**
Muitas vezes, desenvolvedores usam a sigla URI (Uniform Resource Identifier) quando falam de endereços na web. Alguns preferem URL (Uniform Resource Locator), e alguns misturam as duas siglas à vontade. 
Resposta 1 (fácil): Uma URL é uma URI. No contexto do desenvolvimento web, ambas as siglas são válidas para falar de endereços na web. As siglas são praticamente sinônimos e são utilizadas dessa forma.
Resposta 2 (mais elaborada): Uma URL é uma URI, mas nem todas as URI's são URL's! Existem URI's que identificam um recurso sem definir o endereço, nem o protocolo. Em outras palavras, uma URL representa uma identificação de um recurso (URI) através do endereço, mas nem todas as identificações são URL's.
Humm ... ficou claro? Não? Vamos dar um exemplo! Existe um outro padrão que se chama URN (Uniform Resource Name). Agora adivinha, os URN's também são URI's! Um URN segue também uma sintaxe bem definida, algo assim urn:cursos:alura:course:introducao-html-css. Repare que criamos uma outra identificação do curso Introdução ao HTML e CSS da Alura, mas essa identificação não é um endereço.


## Aula 02 Acessando diferentes Portas - video 2
Nesta aula, aprendemos sobre as portas em URLs. As portas são usadas para acessar recursos na web através do protocolo HTTP. A maioria dos sites utiliza a porta 80 para HTTP e a porta 443 para HTTPS. Existem outras portas disponíveis para uso, que vão de 1023 até 65535. As portas entre 0 e 1023 são reservadas para serviços padronizados. O projeto AluraBooks utiliza a porta 3000 para o front-end e a porta 8000 para o back-end. Portas com números maiores são geralmente usadas em ambientes de desenvolvimento.


## Aula 02 Entendendo Dominíos - video 3
Nesta aula, o instrutor aborda a parte do servidor em relação aos URLs. Ele explica o conceito de servidor local, utilizando o exemplo do endereço "localhost:3000". Também fala sobre o uso do endereço IP para acessar um site, exemplificando com o endereço IP do Google. O instrutor explica o funcionamento do Sistema de Nomes de Domínios (DNS) e como ele associa um nome de domínio a um endereço IP. Além disso, ele destaca a hierarquia e estrutura dos domínios, explicando os domínios de nível superior (TLD) e os sub-domínios. Por fim, o instrutor explica a composição de uma URL, destacando o protocolo, o endereço IP ou nome de domínio e o caminho da página.
**nslookup nomedodominio.com**
O comando NSLOOKUP solicita informações para Servidores de Domínios da Internet, podendo trabalhar em dois modos. No modo interativo pode-se interagir com vários Servidores de Domínios e com várias máquinas.

## Aula 02 Conclusão - Nessa aula, você aprendeu a:
Identificar uma URL e entender o seu papel no protocolo HTTP;
Configurar URLs para utilizar: protocolos, domínios, portas, e caminhos específicos;
Utilizar a porta padrão nas URLs com o protocolo HTTP;
Usar nomes de domínios (ao invés de endereços IP) para acessar diferentes sites na Web.


## Aula 03 Inspecionando o Protocolo HTTP - video 1
Nesta aula, o professor recapitula o uso do Chrome e do JavaScript como cliente HTTP para acessar servidores back-end e front-end. Ele destaca a importância de analisar as informações obtidas das requisições na aba "Network" do navegador. Em seguida, ele introduz o telnet, uma ferramenta que permite criar uma conexão TCP com outros servidores e fazer requisições HTTP manualmente. O professor mostra como fazer uma requisição GET e uma requisição de login usando o telnet, explicando o formato das mensagens HTTP. Ele também menciona que o telnet é uma ferramenta de baixo nível e que será apresentada uma nova ferramenta chamada Postman nos próximos vídeos.  
**Telnet**  
Criaremos uma conexão TCP com back-end e o TCP será usado pelo HTTP para transportar as mensagens. Abriremos o telnet no terminal e digitaremos as mensagens HTTP como um cliente, semelhante ao navegador.
> - telnet localhost 8000  
> - GET / HTTP/1.1  
O "GET" indica a obtenção de um conteúdo, a barra define que o conteúdo é da página inicial e o "HTTP/1.1" é o nome do protocolo, seguido da versão.

 Na sequência, vamos realizar uma requisição um pouco mais interessante.
Na página inicial do AluraBooks, na parte superior direita, podemos clicar no botão "Login" e inserir nossos dados cadastrados no sistema:  
> E-mail: geo@alura.com.br Senha: 123  
Pressionando o botão "Fazer login", entraremos no sistema, usando o protocolo HTTP. A seguir, vamos explorar como realizar a mesma ação com o telnet.
> - telnet localhost 8000  
> - POST /public/login HTTP/1.1   
    Content-Type: application/json   
    Content-length: 45  
{"email": "geo@alura.com.br", "senha": "123"}   
Analisando o retorno, reparamos que a requisição foi bem-sucedida. A resposta em texto do servidor começa novamente com HTTP/1.1 200 OK e várias configurações. Depois, temos um JSON com um access token, que é o elemento usado para provar que estamos logados. Aprendemos sobre esse assunto mais adiante; por ora, vamos focar em entender o formato das mensagens HTTP.  

> IMPORTANTE: após muitos erros descobri o por que não estava conseguindo colar(um texto) no TERMINAL TELNET, não aceitou CTRL+V, SHIFT+INS. ERA APENAS CLICANDO COM O BOTÃO DIREITO DO MOUSE, DENTRO DO TERMINAL para colar o texto  
Sem contar que o ENTER tem quer ser prescionado duas vezes para enviar o comando


## Aula 03 Depurando métodos HTTP - video 2
Nesta aula, o instrutor continua explorando o formato dos cabeçalhos de requisições HTTP. Ele utiliza o Postman, uma ferramenta para testar servidores HTTPs e APIs, para demonstrar como criar requisições GET e POST. O instrutor explica que o método GET é utilizado para obter informações de uma página, enquanto o método POST é utilizado para enviar informações, como no caso de um login. Ele menciona também outros métodos HTTP comuns, como PUT e DELETE, que permitem realizar operações em aplicações. O instrutor menciona o acrônimo CRUD, que representa as operações de criar, ler, atualizar e apagar elementos. No próximo vídeo, será explorado o que pode ser feito com o token de acesso recebido após o login.


> **REQUEST** - é uma requisição(solicitação) do cliente ao servidor

> **RESPONSE** - É a resposta do servidor a requisição


## Aula 03 Configurando cabeçalhos para autenticar o usuário - video 3
Nesta aula, aprendemos a usar o Postman para fazer requisições HTTP e entendemos os métodos HTTP. Fizemos login no AluraBooks e obtivemos um código de acesso. Aprendemos a configurar os cabeçalhos da requisição no Postman, adicionando a chave "Authorization" e o valor "Bearer" seguido do token. Com isso, conseguimos acessar uma página protegida e obter os dados dos pedidos. Também foi mencionado o uso de sessões e cookies para "lembrar" o servidor.


## Aula 03 Depurando os códigos resposta HTTP - video 4
Nesta aula, foi abordado o tema dos códigos de status no protocolo HTTP. Foi explicado que esses códigos estão organizados em classes, sendo que o primeiro dígito indica a categoria do código. Os códigos iniciados com o número 1 são raramente usados, enquanto os códigos iniciados com o número 2 indicam operações bem-sucedidas. Os códigos iniciados com o número 3 indicam redirecionamentos, os códigos iniciados com o número 4 indicam erros do lado do cliente e os códigos iniciados com o número 5 indicam erros do lado do servidor. Foram citados exemplos de códigos, como o "400 Bad Request", o "401 Unauthorized" e o "500 Internal Server Error". Esses códigos de status ajudam na criação de aplicações fáceis de integrar, facilitando a comunicação entre o back-end e o front-end de uma equipe de tecnologia.

**RFCs**  
RFCs são documentos que definem as regras de um protocolo. Elas são gratuitas na internet e qualquer pessoa pode acessá-las.  
[Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content](https://www.rfc-editor.org/rfc/rfc7231)


## Aula 03 Conclusão - Nessa aula, você a aprendeu a:  
Inspecionar mensagens HTTP no terminal usando o telnet, para verificar que as mensagens trafegadas são baseadas em texto;
Verificar que as mensagens HTTP são divididas em cabeçalho e corpo da mensagem;
Depurar os métodos HTTP usando o Postman, permitindo ler e criar recursos no backend do AluraBooks;
Configurar cabeçalhos em requisições para o backend, permitindo o acesso a conteúdos que exigem que o usuário esteja logado;
Depurar os códigos de resposta HTTP, os quais são divididos em classes, tais como como 2xx (sucesso) e 4xx (erro do cliente).


## Aula 04 Protegendo a WEB com HTTPS - video 1

