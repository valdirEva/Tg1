# TG1 - 5º semestre de BD

 

 

 

Professor da Disciplina: Giuliano Bertoti 

 

 

 

# TG

 

 

 

Aluno: Valdir Evaristo da SIlva Junior- ra 1460281623038
Orientador: nome

 

 

 

Título do TG: Software para gestao de portaria em condominio

 

 

 



 

 

 




 

 

 

# 1. INTRODUÇÃO

Condomínios edilícios, composto por imóveis que contêm áreas de propriedade exclusiva e áreas de uso comum aos demais condôminos em condomínio, são recentes na história, mas vigentes em todas as grandes cidades. Suas origens se deram quando numerosas cidades, no século XX, buscaram melhor aproveitamento do solo, para tornar mais econômico edificações e subsistência de seus habitantes, concentrar nas circunvizinhanças de locais de trabalho tanto operários como familiares, entre outros fatores, a gerar esta modalidade de convivência. 
No Brasil, a primeira referência à propriedade privada conjugada compartilhada remonta ao século XVII com as Ordenações Filipinas: "E se huma casa for de dous senhorios, de maneira que de hum delles seja o sotão, e de outro o sobrado, não poderá aquêle, cujo for o sobrado, fazer janela sobre o portal daquele, cujo for o sotão, ou logea, nem outro edifício algum "(RODRIGUES 2002). Somente em 1928, com o Decreto-Lei nº 5.481/28, edificações passaram a ser vendidas em parte, e a ser propriedade autônoma cada apartamento, suscetível à alienação independente, transcritos ou inscritos no Registro de Imóveis. No contexto deste Decreto, entre demais regulamentações, passou a reger como instalar e funcionar a assembleia de condôminos, eleição do administrador, votações e formas de repartir as despesas inerentes à edificação, acrescido dos direitos e deveres dos condôminos, assim se deu início ao complexo condominial.
Em face de crescente complexidade, assim como cada vez maior número de moradores nos condomínios edilícios, supõe-se que a presença de um administrador experiente no próprio local proporciona maior assertividade e certeza nos processos decisórios, bem como maior estabilidade na organização de seus demais processos para preservação da memória organizacional, além de melhor dirimir conflitos com técnicas adequadas em gestão de pessoas.
Como quase sempre a cultura tende a ser arraigada, mesmo nos que sofrem diretamente as consequências do poder formal, as ferramentas administrativas podem e devem servir de 20 mediadoras, para evidenciar onde convém flexibilizar ou conduzir de forma menos rígida, e preservar os bons resultados com segurança, calcada nos registros bem ordenados e memória organizacional preservada com clareza, promover cordialidade onde haja necessidade de obediência a processos pré-estabelecidos, para evitar assim tanto a coerção quanto o desinteresse dos envolvidos ante as normas e instruções
O condômino Village Marie, localizado no bairro Vila Maria, em São José dos Campos, SP, já é habitado por moradores há 3 anos, mas até o momento não possui nenhum software de gestão, todos cadastros são realizados manualmente em cadernos e armazenados na portaria, gerando dificuldade e lentidão toda vez que se faz  necessário verificar se uma pessoa é realmente é moradora do condomínio, ou qual o numero da vaga de estacionamento correspondente ao apartamento, se o carro é cadastrado em algum apartamento e até o cadastro de prestadores de serviço e visitantes, com essa dificuldade a sindica viu a necessidade de um  sistema de gestão onde seja possível realizar o cadastro dos apartamentos, automóveis , moradores, visitantes e prestadores de serviço e assim o processo  se torne mais eficaz.

## 1.1. Objetivos do Trabalho 
O objetivo geral deste trabalho é criar um software para o gerenciamento de processos rotineiros em um condomínio:
	Cadastro de moradores em seus respectivos apartamentos;
	Consulta de moradores em seus respectivos apartamentos;
	Edição de moradores cadastrados;
	Exclusão de moradores cadastrados.
	Cadastro de veículos em seus respectivos apartamentos e numero da vaga;
	Consulta de veículos cadastrados;
	Edição de veículos cadastrados;
	Exclusão de veículos cadastrados.
	Cadastro de visitantes com numero do apartamento e data da entrada;
	Consulta de visitantes por nome; numero do apartamento ou data da visita;
 Cadastro de prestadores de serviço  com numero do apartamento e data da visita. 
 Consulta de prestadores de serviço pelo nome, numero do apartamento ou data da visita.
### 1.2. Conteúdo do Trabalho
O presente trabalho está estruturado em seis Capítulos, cujo conteúdo é sucintamente apresentado a seguir:
No Capítulo 2 é feita a fundamentação das tecnologias a linguagem de programação que sera em JAVA e o banco de dados em MySql.



 

 



 

 
# 2. FUNDAMENTAÇÃO TÉCNICA
Este capítulo apresenta a fundamentação teórica e os conceitos necessários para o desenvolvimento deste trabalho, bem como apresenta alguns sistemas já existentes relacionados ao problema. 
A seção 2.1 apresenta as tendências tecnológicas, as linguagens de programação e infraestrutura escolhidas para a solução do problema de gestão de condomínios, e a seção 2.2 traz alguns sistemas já conhecidos no mercado que buscam solucionar um pouco deste desafio, a fim de analisá-los e montar uma visão global do cenário atual de gestão de condomínios.
## 2.1. Conceitos adotados
Para o desenvolvimento de aplicações a linguagem adotada por padrão para confecção das páginas Web é a Hypertext Markup Language (HTML), uma linguagem de marcação de texto que é interpretada e processada pelos navegadores, tendo assim suas informações renderizadas na tela do dispositivo do usuário de forma gráfica. Originalmente, a HTML foi projetada principalmente como uma linguagem para descrever semanticamente documentos científicos. Seu design geral, no entanto, permitiu que ela fosse adaptada, nos anos subsequentes, para descrever vários outros tipos de documentos e até mesmo aplicativos (SMITH, 2013). Várias versões da HTML já foram publicadas, sendo a HTML 5 a versão mais recente. Uma das maiores vantagens de desenvolver aplicações baseadas em HTML é sua característica multiplataforma, isto é, tem compatibilidade com dispositivos de diversos sistemas operacionais e diferentes marcas, o que possibilita uma única frente de desenvolvimento e, ao mesmo tempo, garante o alcance a uma parcela consideravelmente maior de usuários. Entretanto, por si só, esta linguagem não oferece um visual gráfico rico e intuitivo. Por isto o desenvolvimento de uma aplicação para esta linguagem faz uso do Cascading Style Sheets (CSS) e do JavaScript (JS).
A CSS é uma linguagem para descrever a renderização de documentos estruturados
(como aqueles criados com a HTML) na tela (ETEMAD; JR.; RIVOAL, 2017) . Trata-se
de um meio para adicionar cores, sombras, bordas e algumas animações, dentre outros
elementos visuais. Com a CSS também é possível garantir responsividade ao documento,
fazendo com que seu conteúdo se adapte ao dispositivo de saída que o está exibindo,
garantindo legibilidade e acessibilidade à aplicação independentemente do tamanho ou
resolução do aparelho do usuário.
A JS é uma linguagem de programação interpretada que pode funcionar diretamente
no dispositivo do usuário, executando funções programadas em tempo real, deixando
o documento mais dinâmico e interativo. Com a JS podemos, por exemplo, validar
formulários, alterar atributos de elementos e capturar eventos.
Apesar da força destas três linguagens, para construir uma aplicação funcional as
páginas precisam ser mais dinâmicas, apresentar informações que mudam de acordo com o
contexto da aplicação e persistir os dados digitados para futuras consultas e processamentos. As páginas HTML exibem apenas conteúdo estático ao usuário, ou seja, independentemente do momento que a página é acessada ou do usuário que está ativo, a informação exibida é sempre a mesma. Para levar conteúdo dinâmico à HTML é necessário usar uma linguagem de servidor que faça um pré-processamento e possa
Para o desenvolvimento de aplicações nestes moldes há uma variedade de linguagens,
e uma das mais conhecidas e difundidas é a Java, uma linguagem de programação orientada a objetos que apresenta alto desempenho e escalabilidade para aplicações na Web (BARISH, 2002). Diferente da maioria das linguagens de programação, que são compiladas para código nativo de máquina, a linguagem Java é compilada para um código que só é interpretado por uma máquina virtual específica, a Java Virtual Machine (JVM).
Quando se trata de um sistema na nuvem, esta interpretação só ocorre no servidor e
o usuário não percebe o processo, pois ele recebe apenas o resultado em HTML desta
execução.
E, finalmente, para completar a aplicação é preciso uma estrutura para persistência
de dados. Para tanto, pode ser usado um Database Management System (DBMS) que
adote o modelo Relacional, uma estrutura de armazenamento que grava os dados de forma
que eles sejam percebidos pelos usuários como tabelas (ROUSSOPOULOS; DELIS, 1991).
Neste modelo, a linguagem Structured Query Language (SQL) é a mais adotada para
efetuar consultas e gravar dados.
Assim, para a construção de uma aplicação completa, que agrade ao usuário em
termos de compatibilidade, usabilidade, interatividade, relevância e consistência, o sistema
será hospedado em um servidor local e construído sob a HTML, melhorado com CSS
e JS, montado dinamicamente com Java e persistido em um banco de dados relacional.

## 2.2. Trabalhos Correlatos
No mercado podemos encontrar alguns sistemas que possuem a mesma proposta
deste projeto, como o SIN (ICONDEV, 2017), um software de gestão de condomínios
desenvolvido pela Icondev, e o Immobile Condomínio (ALTERDATA, 1989), a solução da
Alterdata.
O SIN oferece aos síndicos ou administradoras de condomínio a tecnologia necessária
para gerenciar condomínios com cadastro de usuários, blocos, unidades habitacionais,
condôminos, fornecedores, plano de contas, registros de consumo, contas a pagar e a
receber, caixa e bancos, boletos ou carnês, renegociações, comunicados internos e acessos na portaria. Além disso ele também oferece relatórios e um portal para o condômino.
Dentre os relatórios disponíveis, destacam-se os relatórios de cadastros, livro diário
de lançamentos, demonstrativo de resultado e diversos relatórios financeiros. É possível
optar por salvar tais relatórios ou enviá-los por e-mail, de acordo com a necessidade do
usuário.

![alt text](https://github.com/valdirEva/Tg1/blob/master/figura%201.png)
 
 Figura 1 – Tela da aplicação SIN.

Este sistema possui uma tela principal (Figura 1) com informações centralizadas
do condomínio, trazendo acesso rápido aos saldos de caixa, contas bancárias e contas
contábeis, avisos de contas a pagar, de solicitações de locações de áreas comuns, dentre
outros dados de interesse do síndico. As outras telas são acessíveis através de um menu,
e todas as operações podem ser realizadas através da interface gráfica da aplicação.
A Icondev também tirou proveito de recursos da computação na nuvem para armazenamento dos dados dos clientes. Assim o sistema pode ser utilizado em qualquer
computador conectado à Internet e o síndico não precisa se preocupar com questões como
vírus ou backup, conforme cita a desenvolvedora em sua página (ICONDEV, 2017).
Apesar de bastante completa, esta aplicação possui alguns pontos negativos. Um dos
principais equívocos da desenvolvedora foi não fornecer uma funcionalidade para montagem da previsão orçamentária, uma obrigação legal e com penalidades para o condomínio (REPÚBLICA, 2002). O segundo ponto a ser observado é que, apesar de ter um funcionamento totalmente online, a aplicação exige a instalação de um componente no computador do usuário e, além disso, como este é um software escrito utilizando a linguagem de programação Java, é necessário que o computador tenha a JVM previamente instalada para que o sistema funcione. Esta questão, além de criar uma barreira de dificuldade para os clientes, os impedem de acessar o sistema pela maioria dos smartphones e tablets comercializados no mercado, pois estes requisitos limitam o uso do sistema a computadores. Por fim, apesar de simples e intuitiva, a interface gráfica do sistema não é responsiva, ficando ilegível em dispositivos com visores menores.
O Immobile Condomínio é um software offline desenvolvido para a gestão de rotinas

![alt text](https://github.com/valdirEva/Tg1/blob/master/figura%202.png)


Figura 2 – Tela da aplicação Immobile Condomínio

das administradoras de condomínios residenciais e comerciais, a fim de facilitar o trabalho
realizado e a comunicação entre administradora, condôminos e síndicos. O sistema possui
diversas ferramentas, muitas opções de relatórios, e também conta com uma interface
intuitiva e amigável (Figura 2).
Por uma assinatura à parte, o sistema da Alterdata também pode ser acessado por uma versão online, utilizando-se de virtualização de máquina para oferecer o serviço na nuvem. Este é um serviço adicional onde o usuário vai precisar apenas de um computador para se conectar à Internet para abrir o Alterdata Cloud (ALTERDATA, 2018), que está disponível nos servidores da desenvolvedora e permite ao cliente operar o sistema sem precisar se preocupar com a instalação, backups, custos com manutenção e infraestrutura ou com ataques ao banco de dados, pois a assinatura inclui estas garantias.
A Alterdata também criou um aplicativo para Android e iOS com alguns recursos básicos para os condôminos, como visualização de boletos, avisos e balancetes, além da possibilidade de reservar áreas de lazer do condomínio. retornar, a cada requisição distinta, um conteúdo HTML diferente, quando necessário.

# 3. DESENVOLVIMENTO
Este capítulo apresenta em detalhes a metodologia e as tecnologias utilizadas para
o desenvolvimento deste trabalho.
A seção 3.1 descreve passo-a-passo a modelagem da aplicação, desde o levantamento
dos atores e requisitos à modelagem do banco de dados, e a seção 3.2 apresenta os frameworks, ferramentas e serviços escolhidos para a concepção do projeto.

## 3.1. Arquitetura do Sistema
A modelagem é uma das principais atividades que levam à criação de um bom software. A modelagem de software utiliza vários modelos que “ajudam a visualizar o sistema como ele é ou como desejamos que ele seja; permitem especificar a estrutura ou o comportamento de um sistema; proporcionam um guia para a construção do sistema; e documentam as decisões tomadas no projeto” (RUMBAUGH; JACOBSON; BOOCH, 2005).
Dentre todos os modelos existentes, os atores, os requisitos do sistema, um caso de uso e um modelo de dados foram escolhidos para ajudar a compreender melhor o sistema elaborado.

## 3.1.1 Atores
Controlador de acesso: é o usuário que controla a entrada e saída de todas pessoas e veículos do condomínio, possui um cadastro e credencial de usuário para autenticação. Ele poderá utilizar as funcionalidades de negócio do sistema, exceto para criar novos usuários do sistema ou excluir qualquer dado. 
Síndico: é o usuário principal do sistema. Ele acessa o painel do condomínio e todas as funcionalidades disponíveis para gerenciar o condomínio. 

## 3.1.2 Modelo de Dados
A modelagem do banco de dados é um passo crucial para o desenvolvimento. Definir as entidades e seus atributos, bem como as as relações ou dependências entre elas é a base para a criação do banco de dados e de toda lógica computacional envolvida na persistência
e recuperação das informações. Um banco de dados mal estruturado pode dificultar a gravação e a recuperação de informações, gerar consultas repetitivas e demoradas, duplicar
informações e até mesmo comprometer a sua integridade.
Após montado, um esquema relacional precisa passar por um processo de normalização
para identificar erros. Estas regras visam reduzir a redundância de dados e aumentar a sua integridade e desempenho (ELMASRI; NAVATHE, 2011). Para ser considerado adequado,
o esquema relacional deve ser analisado e adaptado a cada Forma Normal (FN) a seguir:
❏ 1a FN: todos os atributos de uma entidade precisam ser atômicos e monovalorados,
o que significa que uma tabela não pode ter grupos de repetição.
❏ 2a FN: os atributos não chave de uma entidade devem depender unicamente de
sua chave primária.
❏ 3a FN: os atributos não chave de uma entidade devem ser funcionalmente independentes
uns dos outros.

## 3.2 Tecnologias Utilizadas 
Para o desenvolvimento de uma aplicação de sucesso é preciso estar atento aos passos
tecnológicos tomados pelo mercado. Um sistema, para ser bem colocado, consiste não
somente em um software funcional e que atenda aos requisitos, mas também que possua
um código fonte estruturado, de fácil compreensão e manutenção, além de fácil escalabilidade,
maior segurança e total integridade da informação. No sentido de facilitar estas características, a comunidade de desenvolvedores e empresas de tecnologia tem criado e
mantido inúmeras ferramentas para apoiar o desenvolvimento de aplicações. Neste trabalho procurou aproveitar-se destas tecnologias para trazer ao projeto uma qualidade mais próxima ao que é criado hoje pelas empresas de desenvolvimento, tendo uma estrutura bem conhecida pelos profissionais da área, além de segurança e integridade garantidas pelas ferramentas adotadas.

### 3.2.1. Spring Web MVC
O módulo Spring Web MVC (PIVOTAL, 2018f), como o próprio nome já declara,
traz consigo a estrutura do padrão de arquitetura Model-View-Controller (MVC), já dispensando o programador de mais esta tarefa no desenvolvimento. Outra vantagem deste módulo é a conversão de dados enviados através de formulários Web. Em um cenário padrão, quando o desenvolvedor recebe dados de um formulário, tudo é interpretado como texto, inclusive datas e valores numéricos — já que este é o comportamento do Hypertext Transfer Protocol (HTTP) — e o programador precisa realizar a conversão de cada uma das entradas manualmente. Com esta ferramenta os dados já são convertidos de acordo com o tipo das variáveis que os recebem, sem necessidade de código adicional. Indo ainda mais longe, o módulo é capaz de instanciar objetos inteiros a partir da submissão de um formulário. Por exemplo: suponha a classe Morador com os atributos nome, idade e sexo, e também imagine um formulário de cadastro com os mesmos campos, ao receber os dados deste formulário é possível optar por receber uma instância da classe Morador, já com todos os atributos preenchidos, ao invés de ler cada variável separadamente
para construir um objeto deste tipo.

 ![alt text](https://github.com/valdirEva/Tg1/blob/master/figura%203.png)
 
					Figura3 – Modelo Web MVC 

Na figura 3 podemos ver o Model onde se encontram as entidades que se comunicam com o Service , o Controller onde se encontram os controladores que fazem a comunicação entre a View e o Service.





### 3.2.1.2 Spring Boot
Com todos estes módulos e possibilidades de personalização oferecidos pelo Spring,
uma central de configuração do projeto se torna indispensável. O intuito do Spring Boot
(PIVOTAL, 2018a) é facilitar a criação de projetos, sua configuração e, ainda, sua execução.
Com este módulo, várias configurações que precisariam ser especificadas pelo desenvolvedor em cada um dos outros módulos são centralizadas em um único local ou até
mesmo automatizadas, trazendo clareza e facilitando a criação do projeto. Mas a mais
importante funcionalidade do Spring Boot é vista na fase de implantação do sistema, onde
há possibilidade de criar aplicações autossuficientes (stand-alone) com poucas instruções.
No modelo tradicional, para executar uma aplicação Java é necessário que a máquina possua uma JVM. Uma aplicação Java para Web precisa de um servidor provendo Web Containers e Enterprise JavaBeans (EJB) Containers, como o Apache (APACHE,
2018). Com o Spring Boot estes requisitos são dispensados, pois ele é capaz de encapsular dentro do próprio pacote o interpretador necessário, tornando o software autossuficiente
e facilitando, também, sua distribuição.


### 3.2.1.3 Spring Security
O Spring Security (PIVOTAL, 2018e) é o bloco responsável pelo gerenciamento de
usuários, incluindo a cifragem de senhas, autenticação, sessões e autorização através de
papéis, além de fornecer proteção contra diversos ataques à aplicação. Todos os aspectos deste módulo são configuráveis, como o tempo da sessão, o algoritmo de cifragem das senhas e também as chamadas que podem ser realizadas por determinado papel de usuário a métodos, objetos e, principalmente, requisições Web, pois graças à sua integração com o Spring Web MVC visto na seção 3.2.1.1, antes de atender a uma requisição Web o controlador irá verificar junto a este módulo se o usuário da sessão atual possui tal permissão. Com este componente a aplicação também fica protegida contra ataques como Cross- Site Request Forgery (CSRF), Session Fixation, Clickjacking, dentre outros, pois o sistema irá analisar cada requisição e barrar grande parte do conteúdo malicioso.

 ![alt text](https://github.com/valdirEva/Tg1/blob/master/figura%204.png)
                                       
					Figura 4- Modelo de classes de segurança.

### 3.2.1.4 Spring Data
A persistência de dados pode ser um processo trabalhoso e repetitivo para a comunidade,
uma vez que a programação é orientada a objetos e o banco de dados é relacional e formado por tabelas. Uma série de códigos em SQL precisa ser misturada à logica da
aplicação, e para executá-los é necessário gerenciar uma conexão com o banco de dados,
manipular objetos de consulta e os seus resultados. Para minimizar este esforço a comunidade desenvolveu a tecnologia Object Relational Mappers (ORMs), frameworks capazes de mapear um objeto a uma tabela, bem como as relações entre eles, dispensando a utilização de códigos SQL nativos e manipulação direta de consultas e resultados, além de controlar conexões e transações. Esta iniciativa, entretanto, veio despadronizada e dificultava a migração de um ORM para outro, uma vez que os modelos eram incompatíveis. Com isto surgiu o Java Persistence API (JPA), uma Interface de Programação de Aplicativos, do inglês Application Programming Interface (API), com o intuito de padronizar tais frameworks de persistência de dados. Em um projeto Spring, o Spring Data (PIVOTAL, 2018b) tem por objetivo facilitar o trabalho com a persistência de dados de uma forma geral, em qualquer tipo de base de dados, desde os tradicionais modelos relacionais às base de dados Not Only SQL (NoSQL). Dentro deste módulo há um sub-componente chamado Spring Data JPA (PIVOTAL, 2018c), que é uma abstração da API JPA e visa facilitar ainda mais o seu uso pelo desenvolvedor em um projeto Spring, trazendo suporte ao JPA para todo o ambiente de maneira integrada.
Estas adições trazem ao projeto vantagens como interfaces prontas para CRUD, criação automática de consultas com base no nome do método, possibilidade de paginação
dos resultados, conversão de tipos entre a aplicação e o banco de dados, validação de dados, prevenção contra ataques como o SQL Injection, dentre outros recursos.
Entretanto, como o JPA é apenas uma especificação, e o Spring Data JPA é apenas
um pacote para integrar, dar suporte e facilitar o uso do JPA no ambiente Spring, uma
implementação da API propriamente dita ainda se faz necessária. Desta forma, o ORM
Hibernate (REDHAT, 2018) é adotado para implementar todos estes recursos. Este
framework foi um dos criados pela comunidade e que depois padronizou-se à JPA, sendo
hoje um dos mais adotados no mundo.

 ![alt text](https://github.com/valdirEva/Tg1/blob/master/figura%205.png)

					Figura 5 – Modelo de utilização de spring data

Na figura 4 podemos verificar a utilização do spring security na linha 65 passando os tipos de autorizações que podem utilizar o método atualizaMorador, e na linha 67 é realizado um save do objeto morador no banco de dados, sem precisar especificar cada atributo, o spring data já faz esse serviço e salva corretamente cada campo no banco de dados.



 # REFERÊNCIAS


 ALTERDATA. SOFTWARE PARA GESTÃO DE CONDOMÍNIO - IMMOBILE. 1989.
<HTTPS://WWW.ALTERDATA.COM.BR/IMMOBILE/CONDOMINIO>.(ACCESSADO EM 21/05/2020).

APACHE. WELCOME TO THE APACHE SOFTWARE FOUNDATION! 2018. <HTTPS:
//WWW.APACHE.ORG/>. (ACCESSADO EM 15/11/2018).

BARISH, G. BUILDING SCALABLE AND HIGH-PERFORMANCE JAVA WEB APPLICATIONS
USING J2EE TECHNOLOGY. PUB-AW:ADR: ADDISON-WESLEY, 2002. XVIII + 392 P. ISBN
0-201-72956-3.

ELMASRI, R.; NAVATHE, S. SISTEMAS DE BANCO DE DADOS. [S.L.]: PEARSON
BRASIL, 2011. ISBN 9788579360855.

ETEMAD, E.; JR., T. A.; RIVOAL, F. CSS SNAPSHOT 2017. [S.L.], 2017.
HTTPS://WWW.W3.ORG/TR/2017/NOTE-CSS-2017-20170131/. (ACCESSADO EM 21/05/2020).

ICONDEV. SIN - SISTEMA DE GESTÃO DE CONDOMÍNIOS. 2017. <HTTP:
//WWW.SISTEMACONDOMINIOONLINE.COM.BR/INDEX.HTML>. (ACCESSADO EM 21/05/2020).

PIVOTAL. SPRING BOOT. 2018. <HTTPS://SPRING.IO/PROJECTS/SPRING-BOOT>. (ACCESSADO
EM 01/06/2020).
. SPRING DATA. 2018. <HTTPS://SPRING.IO/PROJECTS/SPRING-DATA>. (ACCESSADO EM
01/06/2020).
. SPRING DATA JPA. 2018. <HTTPS://SPRING.IO/PROJECTS/SPRING-DATA-JPA>.
(ACCESSADO EM 01/06/2020).
. SPRING FRAMEWORK. 2018. <HTTPS://SPRING.IO/PROJECTS/SPRING-FRAMEWORK>.
(ACCESSADO EM 01/06/2020).
. SPRING SECURITY. 2018. <HTTPS://SPRING.IO/PROJECTS/SPRING-SECURITY>.
(ACCESSADO EM 01/06/2020).
. SPRING WEB MVC. 2018. <HTTPS://DOCS.SPRING.IO/SPRING/DOCS/CURRENT/
SPRING-FRAMEWORK-REFERENCE/WEB.HTML>. (ACCESSADO EM 01/06/2020).
PROVOS, N.; MAZIERES, D. USENIX ANNUAL TECHNICAL CONFERENCE. 1999.
<HTTPS://WWW.USENIX.ORG/LEGACY/EVENT/USENIX99/PROVOS/PROVOS_HTML/INDEX.HTML>.
(ACCESSADO EM 01/06/2020).

REPÚBLICA, P. D. LEI NO 4.591, DE 16 DE DEZEMBRO DE 1964. 1964.
<HTTP://WWW.PLANALTO.GOV.BR/CCIVIL_03/LEIS/L4591.HTM>. (ACCESSADO EM 21/05/2020).

RODRIGUES, SILVIO. DIREITO CIVIL - DIREITO DAS COISAS, VOLUME V, ED. SARAIVA, SÃO PAULO, 2002, 27º EDIÇÃO, P.207 - LIVRO I, TIT. 68 § 34

ROUSSOPOULOS, N.; DELIS, A. MODERN CLIENT–SERVER DBMS ARCHITECTURES. SIGMOD,
ACM, V. 20, N. 3, P. 52–61, SET. 1991.

RUMBAUGH, J.; JACOBSON, I.; BOOCH, G. THE UNIFIED MODELING LANGUAGE REFERENCE MANUAL. [S.L.]: ADDISON-WESLEY, 2005. (THE ADDISON-WESLEY OBJECT
TECHNOLOGY SERIES, V. 1). ISBN 9780321245625.

SMITH, M. HTML: THE MARKUP LANGUAGE (AN HTML LANGUAGE REFERENCE).
[S.L.], 2013. HTTP://WWW.W3.ORG/TR/2013/NOTE-HTML-MARKUP-20130528/. (ACCESSADO
EM 21/05/2020).



 


