---
title: Fundamentos da documentação do Git e do GitHub
seo-title: Fundamentos da documentação do Git e do GitHub
description: Este artigo mostra uma visão geral do repositório Git, do repositório GitHub, como o conteúdo é organizado e as convenções de nomenclatura usadas para a documentação da Adobe.
seo-description: este artigo mostra uma visão geral do repositório Git, do repositório GitHub, como o conteúdo é organizado e as convenções de nomenclatura usadas para a documentação da Adobe.
translation-type: ht
source-git-commit: 223b40e1903c5de90dee90a138967efb02237a42

---

# Fundamentos da documentação do Git e do GitHub

## Visão geral

Se você precisar apenas fazer pequenas alterações de texto nos artigos, não será necessário compreender os detalhes deste artigo. Este artigo descreve o fluxo de trabalho para fazer grandes edições, como criar novos artigos, adicionar imagens ou fazer edições contínuas na documentação da Adobe.

Como um colaborador de conteúdo para a documentação da Adobe, você pode interagir com várias ferramentas e processos. Você pode trabalhar em paralelo com outros colaboradores no mesmo projeto, potencialmente no mesmo conteúdo, ao mesmo tempo. Tudo isso é possibilitado pelo software Git e GitHub.

O Git é um sistema de controle de versão aberto que permite colaboração. Vários colaboradores podem trabalhar nos arquivos dos *repositórios*.

O GitHub é um serviço de hospedagem baseado na web para repositórios Git, como aqueles usados para armazenar conteúdo do[docs.adobe.com](https://docs.adobe.com). Para qualquer projeto, o GitHub hospeda o repositório principal, do qual os colaboradores podem fazer cópias para seu próprio trabalho.

## Git

O Git apresenta um fluxo de trabalho de contribuição e uma terminologia exclusiva para dar suporte ao seu modelo distribuído. Por exemplo, não há o bloqueio de arquivos normalmente associado a operações de check-out/check-in. O Git permite que as alterações sejam resolvidas em um nível ainda mais elevado, comparando os arquivos byte por byte.

O Git também usa uma estrutura em camadas para armazenar e gerenciar o conteúdo de um projeto:

- *Repositório*: também conhecido como *repo*, esta é a unidade mais elevada de armazenamento. Um repositório contém uma ou mais ramificações.
- *Ramificação*: todos os repositórios contêm uma ramificação padrão (em geral, chamada de "mestre") e uma ou mais ramificações destinadas a serem mescladas à ramificação mestre. A ramificação mestre serve como a versão atual e a fonte da qual o conteúdo é publicado. É a ramificação principal da qual todas as outras ramificações no repositório são criadas.

Os colaboradores interagem com o Git para atualizar e manipular repositórios nos níveis locais e do GitHub:

- Localmente, por meio de ferramentas como o GitHub Desktop.
- Por meio de [www.github.com](https://www.github.com), que integra o Git para gerenciar a reconciliação das contribuições que retornam ao repositório principal.

## GitHub

Todos os fluxos de trabalho começam e terminam no nível do GitHub, onde o repositório principal de qualquer projeto de documentação da Adobe é armazenado. As cópias que os contribuidores criam para uso próprio estão distribuídas em vários computadores. Essas cópias são eventualmente reconciliadas no repositório GitHub principal do projeto.

### Organização do diretório

A ramificação padrão/mestre de um projeto serve como a versão atual do conteúdo do projeto. O conteúdo da ramificação mestre - e das ramificações criadas a partir dela - está alinhado com a organização dos tópicos do artigo. Os subdiretórios são usados para organizar os ativos de conteúdo e imagem.

Normalmente, é possível encontrar um diretório principal `help` fora da raiz do repositório. O diretório de artigos contém um conjunto de subdiretórios. Os artigos nos subdiretórios são formatados como arquivos Markdown que usam a extensão *.md*.

Na raiz desse diretório, é possível encontrar artigos gerais relacionados a um serviço ou produto geral. Geralmente, é possível encontrar outra série de subdiretórios que correspondem aos recursos/serviços ou cenários comuns.

### Diretório de ativos

Os diretórios do guia do usuário contêm subdiretórios `/assets` para arquivos de imagem referenciados em um diretório.

<!---
### Markdown file template

For convenience, the root directory of each repository typically contains a Markdown template file named `template.md`. You can use this template file as a "starter file" if you need to create a new article for submission to the repository. The file contains:

- A **metadata header** at the top of the file, delineated by two, 3-hyphen lines. It contains the various tags used for tracking information related to the article. It also includes SEO optimizations and reporting processes that Adobe uses to evaluate the performance of the content. So the metadata is important!
- Various **examples of using Markdown** to format the elements of an article.
- General **instructions on the use of Markdown extensions**, which you can use for various types of alerts.
- Examples of **embedding video** by using an iframe.
- General **instructions on the use of docs.adobe.com extensions**, which you can use for special controls such as buttons and selectors.
-->

## Solicitações de pull

Uma *solicitação de pull* fornece uma maneira conveniente para um colaborador propor um conjunto de alterações que serão aplicadas à ramificação padrão. As alterações (também conhecidas como *confirmações*) são armazenadas na ramificação do colaborador, portanto, o GitHub pode primeiro modelar o impacto da *mesclagem* na ramificação padrão. Uma solicitação de pull também serve como um mecanismo para fornecer ao colaborador feedback do processo de compilação/validação - do revisor da solicitação de pull - para resolver possíveis problemas ou perguntas antes que as alterações sejam mescladas na ramificação padrão.

Há duas maneiras de contribuir usando uma solicitação de pull, dependendo do tamanho das alterações que você deseja propor. Abordaremos isso posteriormente, na seção sobre o [fluxo de trabalho do GitHub](local-repo.md) neste guia.
