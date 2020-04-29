---
template: post
title: Conceitos NodeJS
slug: Conceitos NodeJS
draft: true
date: 2020-04-29T00:23:05.369Z
description: Iniciando os estudos do NodeJS
category: 'GoStack, Backend com NodeJS'
tags:
  - nodejs
  - gostack
---
![https://miro.medium.com/max/4000/1*aeWo6e6FC8InJwBl3TmpDw.jpeg](https://miro.medium.com/max/4000/1*aeWo6e6FC8InJwBl3TmpDw.jpeg)

# O que é Node.JS?

* Javascript no back-end;

    *O backend é aquilo que o usuário não enxerga. Quando a gente fala de backend é a camada de negócio da aplicação, integração com serviços de terceiros. O node permite a gente usar o javascript tanto no frontend quando no backend.* 

  * Não lidamos com eventos do usuário final;

      *Como clicar botão.*
  * Rotas e integrações;

      *É assim que ouvimos o que o usuário está pedindo.*
* Plataforma(não lingagem);

    *A linguagem é Javascript, o node é uma plataforma de desenvolvimento.*
* Construída em cima da V8;

     *A máquina que roda por trás do chrome. O Node usa esse motor para rodar o JS no backend.*
* Comparável com PHP / Ruby / Python / Go;

    *Tem vantagens a algumas linguagens mais tradicionais.*

![https://miro.medium.com/max/548/1*o474X_2eTiF2Dnn39h6Rjg.jpeg](https://miro.medium.com/max/548/1*o474X_2eTiF2Dnn39h6Rjg.jpeg)

# O que é o NPM?

* Instalar bibliotecas de terceiros;

    *Gerenciador de pacote, permite que instale ferramentas de terceiros, instala uma biblioteca para facilitar esse desenvolvimento.*
* Fornece bibliotecas;

    *Fornece Bibliotecas para que terceiros utilizem as nossas bibliotecas criadas.*
* Por que utilizaremos o Yarn?

    *O yarn é mais rápido e mais desenvolvido que o NPM.* 
* Comparável ao: Composer do PHP, Gems do Ruby, PIP do Python

# Características do Node

* Arquitetura Event-loop;

*É uma arquitetura totalmente baseada em **eventos**. Um ponto muito importante é a **Call Stack**.*

* A Call Stack;

    *Pilha de eventos, um evento pode ser vista como uma função que o node processa em um loop eterno rodando na nossa aplicação sem parar vendo se tem uma nova função que foi disparada e executa em formato de pilha.*
* Node single-thread;

    *Ele executa apenas em uma thread do processador, o processo dele vai ficar alocado em um core do processamento.*

  * C++ por tŕas com libuv;

      *O node usa essa biblioteca do libuv permite usar multi-threads do processador para agilizar o processamento. Então por debaixo dos panos, o node usa multi-threads.*
  * Background threads;
* Non-blocking I/O

    *Ele tem uma arquitetura Non-blocking I/O, isso quer dizer que quando fazemos uma requisição para o Node, não precisa retornar todos os dados de uma só vez, podemos retornar em parte, pois não iremos bloquear outras requisições. A conexão não é perdida, podemos ter assim aplicações em tempo real, a requisição fica aberta.*

![https://www.tgmarinho.com/static/5cac3789a6a8ba041175c2edc675213b/16abd/call_stack_node.png](https://www.tgmarinho.com/static/5cac3789a6a8ba041175c2edc675213b/16abd/call_stack_node.png)

*A call stack é nada mais que uma ilha. A partir do momento que executamos uma função ela vai para dentro da call stack, vamos chamando outras funções, o event loop monitora essa call stack, e vai  pegar função por função executando em multi-threads usando a biblioteca libuv. A stack é realmente uma pilha, ou seja é last in, first out - SEMPRE -*

# Frameworks

![https://miro.medium.com/max/805/1*alZcSIb0lcN7gQIx2tJ_tg.png](https://miro.medium.com/max/805/1*alZcSIb0lcN7gQIx2tJ_tg.png)

*Framewors sem opinião, ótimo para quem está começando agora, ótimo para micro-serviços*

![https://carlosdevcode.files.wordpress.com/2017/02/adonis-topo.png?w=656](https://carlosdevcode.files.wordpress.com/2017/02/adonis-topo.png?w=656)

*Framework mais robusto e mais opinado, além de ser mais produtivos que tem hoje em dia.*

![https://www.hiago.me/wp-content/uploads/2018/05/NestJSWalpappers-520x245.png](https://www.hiago.me/wp-content/uploads/2018/05/NestJSWalpappers-520x245.png)

*Framework mais robusto e mais opinado, porém está começando a crescer agora.*

Support