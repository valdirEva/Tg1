# TG1 - 5º semestre de BD

 

 

 

Professor da Disciplina: Giuliano Bertoti 

 

 

 

# TG

 

 

 

Aluno: Valdir Evaristo da SIlva Junior- ra 1460281623038
Orientador: nome

 

 

 

Título do TG: Software para gestao de portaria em condominio

 

 

 



 

 

 


# 1ª Quinzena de maio

 

 

 

## 1. INTRODUÇÃO

Condomínios edilícios, composto por imóveis que contêm áreas de propriedade exclusiva e áreas de uso comum aos demais condôminos em condomínio, são recentes na história, mas vigentes em todas as grandes cidades. Suas origens se deram quando numerosas cidades, no século XX, buscaram melhor aproveitamento do solo, para tornar mais econômico edificações e subsistência de seus habitantes, concentrar nas circunvizinhanças de locais de trabalho tanto operários como familiares, entre outros fatores, a gerar esta modalidade de convivência. 
No Brasil, a primeira referência à propriedade privada conjugada compartilhada remonta ao século XVII com as Ordenações Filipinas: "E se huma casa for de dous senhorios, de maneira que de hum delles seja o sotão, e de outro o sobrado, não poderá aquêle, cujo for o sobrado, fazer janela sobre o portal daquele, cujo for o sotão, ou logea, nem outro edifício algum "(RODRIGUES 2002). Somente em 1928, com o Decreto-Lei nº 5.481/28, edificações passaram a ser vendidas em parte, e a ser propriedade autônoma cada apartamento, suscetível à alienação independente, transcritos ou inscritos no Registro de Imóveis. No contexto deste Decreto, entre demais regulamentações, passou a reger como instalar e funcionar a assembleia de condôminos, eleição do administrador, votações e formas de repartir as despesas inerentes à edificação, acrescido dos direitos e deveres dos condôminos, assim se deu início ao complexo condominial.
Em face de crescente complexidade, assim como cada vez maior número de moradores nos condomínios edilícios, supõe-se que a presença de um administrador experiente no próprio local proporciona maior assertividade e certeza nos processos decisórios, bem como maior estabilidade na organização de seus demais processos para preservação da memória organizacional, além de melhor dirimir conflitos com técnicas adequadas em gestão de pessoas.
Como quase sempre a cultura tende a ser arraigada, mesmo nos que sofrem diretamente as consequências do poder formal, as ferramentas administrativas podem e devem servir de 20 mediadoras, para evidenciar onde convém flexibilizar ou conduzir de forma menos rígida, e preservar os bons resultados com segurança, calcada nos registros bem ordenados e memória organizacional preservada com clareza, promover cordialidade onde haja necessidade de obediência a processos pré-estabelecidos, para evitar assim tanto a coerção quanto o desinteresse dos envolvidos ante as normas e instruções
O condômino Village Marie, localizado no bairro Vila Maria, em São José dos Campos, SP, já é habitado por moradores há 3 anos, mas até o momento não possui nenhum software de gestão, todos cadastros são realizados manualmente em cadernos e armazenados na portaria, gerando dificuldade e lentidão toda vez que se faz  necessário verificar se uma pessoa é realmente é moradora do condomínio, ou qual o numero da vaga de estacionamento correspondente ao apartamento, se o carro é cadastrado em algum apartamento e até o cadastro de prestadores de serviço e visitantes, com essa dificuldade a sindica viu a necessidade de um  sistema de gestão onde seja possível realizar o cadastro dos apartamentos, automóveis , moradores, visitantes e prestadores de serviço e assim o processo  se torne mais eficaz.

### 1.1. Objetivos do Trabalho 
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



 

 

# 2ª Quinzena de maio

 

 
## 2. FUNDAMENTAÇÃO TÉCNICA
Este capítulo apresenta a fundamentação teórica e os conceitos necessários para o desenvolvimento deste trabalho, bem como apresenta alguns sistemas já existentes relacionados ao problema. 
A seção 2.1 apresenta as tendências tecnológicas, as linguagens de programação e infraestrutura escolhidas para a solução do problema de gestão de condomínios, e a seção 2.2 traz alguns sistemas já conhecidos no mercado que buscam solucionar um pouco deste desafio, a fim de analisá-los e montar uma visão global do cenário atual de gestão de condomínios.
### 2.1. Conceitos adotados
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

### 2.2. Trabalhos Correlatos
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

![alt text](http://url/to/figura 1.png)
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

 Figura 2 – Tela da aplicação Immobile Condomínio

das administradoras de condomínios residenciais e comerciais, a fim de facilitar o trabalho
realizado e a comunicação entre administradora, condôminos e síndicos. O sistema possui
diversas ferramentas, muitas opções de relatórios, e também conta com uma interface
intuitiva e amigável (Figura 2).
Por uma assinatura à parte, o sistema da Alterdata também pode ser acessado por uma versão online, utilizando-se de virtualização de máquina para oferecer o serviço na nuvem. Este é um serviço adicional onde o usuário vai precisar apenas de um computador para se conectar à Internet para abrir o Alterdata Cloud (ALTERDATA, 2018), que está disponível nos servidores da desenvolvedora e permite ao cliente operar o sistema sem precisar se preocupar com a instalação, backups, custos com manutenção e infraestrutura ou com ataques ao banco de dados, pois a assinatura inclui estas garantias.
A Alterdata também criou um aplicativo para Android e iOS com alguns recursos básicos para os condôminos, como visualização de boletos, avisos e balancetes, além da possibilidade de reservar áreas de lazer do condomínio. retornar, a cada requisição distinta, um conteúdo HTML diferente, quando necessário.

 ## REFERÊNCIAS


 ALTERDATA. SOFTWARE PARA GESTÃO DE CONDOMÍNIO - IMMOBILE. 1989.
<HTTPS://WWW.ALTERDATA.COM.BR/IMMOBILE/CONDOMINIO>.(ACCESSADO EM 21/05/2020).

BARISH, G. BUILDING SCALABLE AND HIGH-PERFORMANCE JAVA WEB APPLICATIONS
USING J2EE TECHNOLOGY. PUB-AW:ADR: ADDISON-WESLEY, 2002. XVIII + 392 P. ISBN
0-201-72956-3.

ETEMAD, E.; JR., T. A.; RIVOAL, F. CSS SNAPSHOT 2017. [S.L.], 2017.
HTTPS://WWW.W3.ORG/TR/2017/NOTE-CSS-2017-20170131/. (ACCESSADO EM 21/05/2020).

ICONDEV. SIN - SISTEMA DE GESTÃO DE CONDOMÍNIOS. 2017. <HTTP:
//WWW.SISTEMACONDOMINIOONLINE.COM.BR/INDEX.HTML>. (ACCESSADO EM 21/05/2020).

REPÚBLICA, P. D. LEI NO 4.591, DE 16 DE DEZEMBRO DE 1964. 1964.
<HTTP://WWW.PLANALTO.GOV.BR/CCIVIL_03/LEIS/L4591.HTM>. (ACCESSADO EM 21/05/2020).

RODRIGUES, SILVIO. DIREITO CIVIL - DIREITO DAS COISAS, VOLUME V, ED. SARAIVA, SÃO PAULO, 2002, 27º EDIÇÃO, P.207 - LIVRO I, TIT. 68 § 34

ROUSSOPOULOS, N.; DELIS, A. MODERN CLIENT–SERVER DBMS ARCHITECTURES. SIGMOD,
ACM, V. 20, N. 3, P. 52–61, SET. 1991.

SMITH, M. HTML: THE MARKUP LANGUAGE (AN HTML LANGUAGE REFERENCE).
[S.L.], 2013. HTTP://WWW.W3.ORG/TR/2013/NOTE-HTML-MARKUP-20130528/. (ACCESSADO
EM 21/05/2020).


 

# 1ª Quinzena de junho
 
(coloque aqui tudo que você fez referente ao capítulo 3 no formato exato de BD)

 

 

 

# 2ª Quinzena de junho

 

 

 

(coloque aqui tudo que você fez referente ao capítulo 3 no formato exato de BD) + crie um pasta chamada "Desenvolvimento" e coloque o início do código

 

 

 

# 1ª Quinzena de julho
