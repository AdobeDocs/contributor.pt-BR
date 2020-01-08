---
title: Guia do colaborador para a documentação da Adobe
seo-title: Visão geral do guia do colaborador para a documentação técnica da Adobe Experience Cloud
description: O guia descreve como você pode contribuir com sugestões e adições para o site da documentação da Adobe.
seo-description: O guia descreve como você pode contribuir para a documentação técnica da [!UICONTROL Adobe Experience Cloud].
translation-type: ht
source-git-commit: afcd9363375adbc21a0e9a027d3f5ce59e08cd70

---


# Visão geral do guia do colaborador para a documentação da Adobe

## O que é a Documentação colaborativa

Durante o ano de 2019, todo o conteúdo de documentação técnica e de capacitação da Adobe Experience Cloud está sendo transferido para uma nova plataforma, com base em princípios de código aberto, utilizando as soluções GitHub, Markdown e Adobe Experience Cloud, incluindo o Adobe Experience Manager, Analytics, Launch e Target.

Este modelo de código aberto melhora a qualidade do conteúdo e a comunicação entre clientes, equipes de documentação e equipes de produtos. Em todas as páginas, agora você pode classificar a utilidade do conteúdo, registrar problemas e até mesmo contribuir com sugestões de conteúdo como solicitações de Git (PRs). As equipes de documentação da Adobe monitoram as contribuições e os problemas diariamente, além de fazerem atualizações e ajustes, conforme necessário.

## Trabalhar com documentação colaborativa

Como usuário desse material, independentemente de se você for um funcionário, parceiro, cliente ou até mesmo um cliente potencial, você tem a opção de contribuir para essa documentação de várias maneiras simples:

* classificar o nível de ajuda da página
* registrar um problema em relação a uma página específica
* enviar uma edição rápida para a criação de artigos inteiros, completa com ativos e amostras de código

Este guia descreve tudo o que você precisa saber para interagir e contribuir com esse conjunto de materiais.

<!--
> [!IMPORTANT]
> All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
-->

## Faça edições rápidas nos documentos existentes

Fazer edições rápidas é uma boa maneira de corrigir pequenos erros e omissões nos documentos. Se um artigo exibir um botão Edit (Editar) como mostrado abaixo, você poderá fazer uma correção rápida. Ao editar o documento, você envia uma solicitação de pull (PR) para enviar a correção/sugestão para nós e poderemos vetar, aprovar e publicar a sugestão.

1. Assine o [Contrato de licença de colaborador (CLA)](http://opensource.adobe.com/cla.html) se for aceitável.

   É necessário enviar somente um CLA da Adobe uma vez.
1. Clique em **`Edit this page`** na coluna à direita para ir para o arquivo de origem do Markdown no GitHub.
1. Clique no ícone de lápis para editar o artigo.

   > [!NOTE]
   > Se o ícone de lápis estiver esmaecido, será necessário fazer logon na sua conta GitHub ou criar uma nova conta.

   ![Localização do ícone de lápis](assets/edit-icon.png)

1. Faça as alterações no editor da web. Você pode clicar na guia **Preview changes** (Visualizar alterações) para verificar a formatação da alteração.
1. Depois de fazer as alterações, navegue até a parte inferior da página. Insira um título e uma descrição para a sua PR e clique em **Propose file change** (Propor alteração de arquivo), conforme mostrado na figura a seguir:

   ![como propor sua alteração](assets/submit-pull-request.png)

   >[!NOTE] Se você receber uma mensagem de erro de validação em relação à assinatura de um Contrato de licença de colaborador (CLA), clique em **Detalhes** para abrir o contrato de licença. Assine o contrato, se for aceitável. Em seguida, feche e abra a solicitação de extração e prossiga.

Isso é tudo. Obrigado! Os membros da equipe de documentação analisarão e mesclarão sua solicitação de pull.

## Registrar um problema

Outra maneira fácil de nos informar sobre um problema de conteúdo é usar a opção “Log an Issue” (Registrar um problema).

1. Se você perceber um problema com um conteúdo, clique no link `Log an Issue` no canto inferior direito de qualquer página. Consulte a figura abaixo:

   ![](assets/git_log_issue.png)

   > [!NOTE]
   > Você precisará fazer logon na sua conta GitHub ou criar uma nova conta para registrar um problema.

   Clicar neste link permitirá registrar um tíquete rápido conosco, usando a interface do GitHub Issue.

1. A URL da página com o problema será preenchida automaticamente no campo de descrição. Preencha o título, escreva uma breve descrição do problema e clique em *Submit new issue* (Enviar novo problema).

   ![](assets/git_issue_example.png)

O envio de um problema notificará diretamente a equipe de conteúdo da página que poderá tomar uma ação. Quando atualizarmos o conteúdo, você será informado na interface do GitHub Issues e notificado por e-mail quando o problema for atualizado ou encerrado.

## Compreender as permissões do GitHub

A interface de edição do GitHub se adapta às suas permissões de repositório. As imagens acima são precisas para os colaboradores que não têm permissões de gravação no repositório de destino. O GitHub cria automaticamente uma bifurcação do repositório de destino na sua conta. Se você tiver acesso de gravação no repositório de destino, o GitHub criará uma nova ramificação nele.

A Adobe usa solicitações de pull para todas as alterações, mesmo para colaboradores com acesso de gravação. A maioria dos repositórios protegem a ramificação `master` para que as atualizações sejam enviadas como solicitações de pull.

A experiência de edição no navegador é melhor para pequenas alterações ou alterações pouco frequentes. Se você fizer grandes contribuições ou usar recursos avançados do Git, recomendamos [bifurcar o repositório e trabalhar localmente](setup/full-workflow.md).

## Fornecer feedback

Com um conjunto de soluções tão grande quanto o da Adobe, a documentação está sempre em progresso. Se você detectar erros, registre um problema. Caso tenha sugestões sobre o material, informe-nos. Diga-nos quais informações você estava procurando. Informe-nos se você não conseguiu encontrar o que precisava. Caso tenha dificuldade para concluir sua tarefa, diga-nos como podemos ajudá-lo a aprender sobre nossas soluções.

A equipe de Documentação Colaborativa agradece a todos os autores e produtores de conteúdo da [!UICONTROL Adobe Experience Cloud].
