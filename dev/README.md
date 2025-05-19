# *Onboarding* da frente de desenvolvimento

A ideia principal do *onboarding* de desenvolvimento é que o novo membro seja capaz de aprender/exercitar os conceitos básicos das seguintes ferramentas:

- Kanban
- Git
- Docker
- MySQL
- Spring Boot com Java
- Angular com Typescript
- Android com Kotlin

É importante destacar que toda parte de Android é destinada para aqueles membros que vão trabalhar nos aplicativos do projeto. Os demais tópicos, são destinados ao desenvolvimento e manutenção do sistema web.

Cada um dos tópicos tem sua própria seção que contém links para tutoriais, video aulas e documentação. A ideia é que o novo membro estude e seja capaz de criar um mini-projeto que é descrito no final desse arquivo. Obviamente, o mini-projeto deve ser desenvolvido utilizando as ferramentas descritas neste documento para que o mesmo crie uma base para começar a desenvolver no projeto.


**Nota 1**: o material aqui listado não é definitivo. Nada impede que você busque conhecimento em outras fontes. Inclusive, caso encontre fonte melhores, sinta-se livre para complementar esse *onboarding*.

**Nota 2**: caso você domine um assunto, você pode pular ou assitir de maneira mais rápida apenas para relembrar. Não é porque uma playlist tenha 20h de vídeos, por exemplo, que você é obrigado a assistir tudo. Ninguém melhor do que você mesmo para entender o que precisa ser relembrado ou aprendido.

___

## Kanban
O Kanban é o método de gerenciamento das atividades que utilizamos no projeto. O seu uso é bem simples e você precisa aprender apenas os conceitos básicos. Portanto, assistir o vídeo a seguir é o suficiente:
- [Aprenda Kanban em 9 minutos (Desenvolvimento Ágil de Software)](https://www.youtube.com/watch?v=WjZBnYa58B4)

___

## Git
O Git é parte fundamental para programação em time. Muito provavelmente você já sabe os conceitos básicos. Porém, caso não saiba ou esteja enferrujado no assunto, estude os seguintes materiais:

- [Controle de versão utilizando Git](http://pachecoandre.com.br/assets/files/mini-tutorial-git.pdf)
- Playlist: [Curso de Git para iniciantes](https://www.youtube.com/watch?v=WVLhm1AMeYE&list=PLInBAd9OZCzzHBJjLFZzRl6DgUmOeG3H0)
- [O que é GitFlow](https://www.youtube.com/watch?v=JyyGm4S3YaM)
- [Git Cheat Sheet](https://www.git-tower.com/blog/git-cheat-sheet)

O Gitflow utilizado nos projetos é descrito no [repositório de documentação](https://github.com/life-ufes/docs).


___
## Docker
O docker é utilizado para criar tanto o ambiente de desenvolvimento, quanto o ambiente de produção do sistema web. Se você já domina o assunto, você pode pular os tutoriais e ir direto para a subseção [Criando o ambiente de desenvolvimento](criando-o-ambiente-de-desenvolvimento). 

### *Onboarding* docker

Todos os links para os tutoriais são listados na sequência:

- Básico sobre docker
  - [Tutorial básico sobre docker](http://computacaointeligente.com.br/outros/docker-basico-data-science/)
  - [O mínimo que você precisa saber sobre Docker](https://www.youtube.com/watch?v=ntbpIfS44Gw)

- Básico sobre `Dockerfile`
  - [O que é Dockerfile? (A receita para criação de containers)](https://www.youtube.com/watch?v=5QGexrfqu60)

- Básico sobre `Docker compose`
  - [Docker Compose na prática (Fácil)](https://www.youtube.com/watch?v=HxPz3eLnXZk)

### Criando o ambiente de desenvolvimento
Para criar o ambiente de desenvolvimento é necessário levantar diversos containers. Para treinar essa habilidade, primeiro você pode assistir [essa video aula](https://www.youtube.com/watch?v=c-Bq6JUfRnk).

No projeto que você vai trabalhar, o ambiente de desenvolvimento é criado utilizando o `docker compose`. O arquivo `docker-compose.yml` estará disponível no repositório do projeto. Quando chegar nesse ponto, consulte os demais membros do time para entender como o ambiente de desenvolvimento funciona.


## MySQL
O MySQL é nosso servidor de banco de dados. Neste projeto o banco de dados é gerenciado pelo framework Spring Boot (que será o próximo tópico desse *onboarding*). Ele é quem vai criar as tabelas do banco, gerenciar as entradas, realizar as consultas, etc.

Na maioria das vezes, não será necessário utilizar SQL para realizar consultas. Porém, é importante que você saiba como funciona um banco de dados relacional. Além disso, eventualmente, vamos verificar algo dentro do banco fora do framework. Por conta disso, caso você não saiba nada sobre banco de dados ou está enferrujado no assunto, é recomendável que você estude um pouco sobre o assunto:
- [Playlist com curso completo de MySQL](https://www.youtube.com/watch?v=Ofktsne-utM&list=PLHz_AreHm4dkBs-795Dsgvau_ekxg8g1r)
  - Se você já sabe como funciona, você não precisa assistir todos os videos. Basta avançar e relembrar os principais conceitos

Normalmente, nós utilizamos o PHPMyAdmin para ter uma interface gráfica de gerenciamento do banco de dados. Porém, sinta-se livre para utilizar outra ferramenta, como por exemplo, o MySQL Workbench. 
- [phpMyAdmin: curso rápido em 17 min | MySQL | Insert, Select, Update, Delete, Create table e Backup](https://www.youtube.com/watch?v=kviT7G14gqk)
- [Como usar o MySQL Workbench Fácil e Rápido](https://www.youtube.com/watch?v=IgO6L7jXbxY)

___
## Spring Boot com Java
Spring boot é o framework utilizado no backend do sistema web. Ele é programado em Java e faz toda a lógica de negócio para que o frontend funcione corretamente. O framework torna a construção e manutenção do banco de dados e a construção da API RESTful muito mais fácil. 

Como o framework é programado em Java, a primeira parte dessa seção é revisar ou aprender Java. Consuma o que achar necessário do material a seguir:

- [Programação básica em Java](http://professor.unisinos.br/pjaques/material/java_basico.pdf)
- [Java Crash Course 2022](https://www.youtube.com/watch?v=OBabVd0STLM)

Antes de entrar no Spring Boot propriamente dito, é interessante que você dê uma olhada no padrão Model-View-Control (MVC):
- [Padrão MVC (Model - View - Controller)](https://www.youtube.com/watch?v=mMDt9g7bMjk)

Agora sim, vamos primeiro entender o que é o Spring Boot:
- [Spring Boot: Tudo que você precisa saber!](https://blog.geekhunter.com.br/tudo-o-que-voce-precisa-saber-sobre-o-spring-boot/)
- [O que é Spring Boot e quais as vantagens de usá-lo?](https://www.youtube.com/watch?v=ABjV1bObFW8)

Entendido o que é o Spring Boot, você pode seguir esses tutoriais para criar o primeiro projeto:
- [Spring Quickstart Guide](https://spring.io/quickstart)
- [Building an Application with Spring Boot](https://spring.io/guides/gs/spring-boot/)
- [Building a RESTful Web Service](https://spring.io/guides/gs/rest-service/)
- [Spring Boot | Curso Completo 2022](https://www.youtube.com/watch?v=LXRU-Z36GEU)

É importante ficar claro que o Spring Boot prover diversos mini-frameworks. Talvez, os dois mais importantes para o projeto são:
- [Spring Data JPA](https://docs.spring.io/spring-data/jpa/docs/current/reference/html/): usado para fazer a interface com o banco de dados, no caso, MySQL
- [Spring Data REST](https://docs.spring.io/spring-data/rest/docs/current/reference/html/): usado para fazer toda interface da API HTTP do projeto

Além dos dois citados acima, projeto também utiliza o [Spring Security](https://spring.io/projects/spring-security). Você pode aprender o básico sobre o assunto:
- [Autenticação e Autorização com Spring Security](https://www.youtube.com/watch?v=pkIEV2Yls_8)

Por fim, saiba que a [documentação do Spring Boot](https://spring.io/projects/spring-boot) é excelente e você pode aprender bastante através dela.

**Nota:** a IDE que o time usa para desenvolver com Spring Boot é a [IntelliJ](https://www.jetbrains.com/idea/) usando o Maven como gerenciador de dependências
- Como aluno da universidade, você pode usar o seu e-mail institucional para obter todas as IDEs PRO da JetBrains de maneira gratuita
- Todavia, caso não queira, você pode utilizar a versão community. Ela é mais do que suficiente

___
## Angular
O Angular é framework utilizado para fazer o frontend do sistema. Então primeiro, você precisa entender o que é o Angular:
- [ O que é Angular](https://www.youtube.com/watch?v=Jyj_qIKL_f8)

O Angular é programado usando o Typescript. Sendo assim, é interessante que dê uma olhada nos principais conceitos da linguagem antes de prosseguir:
- [Curso de Typescript na prática - Aprenda Typescript em 1h](https://www.youtube.com/watch?v=lCemyQeSCV8)

Agora, você está mais preparado para encarar uma playlist explicando os principais conceitos do Angular. Porém, o Angular está em constante atualização. Mesmo que você aprenda com uma versão mais antiga, os conceitos bases continuam os mesmo. A seguir existem duas sugestões, você pode escolher qual usar:
- [Curso Angular 13](https://www.youtube.com/playlist?list=PLnDvRpP8Bnex2GQEN0768_AxZg_RaIGmw)
- [Curso Angular com Spring Boot](https://www.youtube.com/watch?v=qJnjz8FIs6Q&list=PLGxZ4Rq3BOBpwaVgAPxTxhdX_TfSVlTcY)

Também existe um [tutorial falando sobre o Angular mais moderno](https://www.youtube.com/watch?v=6jZ0ewVQP0Y&list=PLGxZ4Rq3BOBr-GEzf90FxQWqbskI682o2), que introduziu o conceito de remoção dos módulos.


**Nota:** a IDE que o time usa para desenvolver com Angular é o [VS Code](https://code.visualstudio.com/), que é gratuito tanto para windows, quanto para Linux. Junto ao VS Code, você de instalar os seguintes plugins para aumentar sua produtividade:
- Angular Extension Pack 
- VSCode simpler Icons with Angular
- ESLinter (importante para ter um padrão de códificação)

### Testes com Angular
- Tutorial rápido de como realizar testes com o Angular: [Vídeo](https://www.youtube.com/watch?v=bRkD7aYMbow)
- Documentação necessária: [Jasmine](https://jasmine.github.io/pages/docs_home.html) | [Karma](https://karma-runner.github.io/6.4/config/configuration-file.html)
- Projeto de treinamento feito pelo Rafael para praticar: [Repositório](https://github.com/rsadr0pyz/testing-presentation)  
- Também foi desenvolvido diversos utilitários para acelerar o uso do framework no projeto. Cheque sua documentação [aqui](https://github.com/pad-ufes/docs/blob/main/testing/testes_software.md).
___
## Android com Kotlin
No passado, o aplicativo do projeto era desenvolvido utilizando [React-native](https://reactnative.dev/) para que funcionasse tanto para Android quanto iOS. Porém, atualmente, o app precisa rodar apenas em Tablets Galaxy S6, o que facilita bastante o desenvolvimento, uma vez que sabemos o device alvo. Nesse sentido, o desenvolvimento foi migrado para um app nativo em Android utilizando Kotlin.

Aqui você possui duas opções de fluxo:

1) Você pode utilizar a sequência da disciplina de Desenvolvimento de Aplicativos Móveis do Prof. André Pacheco:
  - [Notas de aula em formato de slides](https://drive.google.com/drive/folders/1WU1O8HL-0y9rUpaUmuyBvp52V3efHG9n?usp=sharing)
  - [Repositório com códigos exemplos](https://github.com/mobile-dev-ufes/material-disciplina)


2) Você pode utililizar os links a seguir:


O primeiro passo para é entender o básico de Android. Para isso, você pode consultar o material a seguir:
- Introdução ao Kotlin
  - [Parte 1](https://docs.google.com/presentation/d/15lj9SM677vVn0s9szQuEELlpZ05dCJZJurZVJOlSYdU/edit?usp=sharing)
  - [Parte 2](https://docs.google.com/presentation/d/1L2JQZrXHqbFjYg2DGAbgAngXhr7X5Y-KwQ45SiIoWPI/edit?usp=sharing)
  - [Parte 3](https://docs.google.com/presentation/d/1tH67owMG48p_7MOT43Ief53WLQzuKM3cuPaYeQLaZm4/edit?usp=sharing)
- Caso prefira assistir uma playlist de videos:
  - [Curso de Kotlin para Iniciantes](https://www.youtube.com/watch?v=hEbb9cckl9c&list=PLM__ueuR0mKD2cSYDNRxSMfOb3EZ2wmFW&index=2)

Na sequência, você pode explorar os conceitos básicos de Android para construir uma aplicação:
- [Android Nativo com Kotlin](https://youtu.be/Ghx79FLbsNA)

Agora, você pode explorar a construção de uma API com o retrofit:
- [Como consumir APIs com Retrofit usando Android e Kotlin](https://youtu.be/U3Nmw0_BMVs)

E por fim, como utilizar o SQLite com o ROOM:
- [Salvar dados em um banco de dados local usando o Room](https://developer.android.com/training/data-storage/room)
- [Room Database: Introdução a Persistência de Dados com Kotlin localmente](https://www.youtube.com/watch?v=JQ_isBkRWzc)



# Mini-projeto de um sistema web
A ideia do mini-projeto é bem simples e aberta. Basicamente, você deve criar um mini-sistema que faça cadastro e consulta de dados utilizando as ferramentas descritas anteriormente. Obviamente, você deve criar o backend com usando Spring Boot e frontend usando angular. Não precisa ser nada sofisticado ou bonito. Foque na funcionalidade. Todavia, o seu sistema deve conter:
- Uma tela de login
- Uma tela de cadastro de dados
- Uma tela de visualização dos dados cadastrados
- Uma tela com pelo menos um filtro dos dados

Para isso, você deve criar uma API RESTful capaz de inserir, atualizar e obter dados. Esses dados devem ser salvos em um banco de dados MySQL.

Algumas ideias de sistema:
- Sistema de cadastro de produto em uma loja
- Sistema de cadastro de pacientes em um hospital
- Sistema de cadastro de itens de um jogo

# Mini-projeto Android
A ideia do mini-projeto Android segue a mesma linha do sistema web. A ideia é criar um aplicativo apenas para exercitar conceitos. Para isso, o seu app deve conter:

- Um projeto criado a partir de um `Navigation Drawer Activity`
- Uma tela de cadastro de dados
- Uma tela de visualização de dados
- Inserção e obtenção de dados via API REST usando o pacote Retrofit
- Salvar dados relevantes usando SQL Lite através do pacote ROOM
- Tirar uma foto e enviar ela usando a API


