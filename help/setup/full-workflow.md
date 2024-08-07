---
title: Fluxo de trabalho de contribuição do GitHub para grandes alterações
description: Saiba como fazer contribuições para a documentação da Adobe na Experience League.
exl-id: ad467ad4-abd2-4166-8659-e29c48d268ec
source-git-commit: a3c283c5c0d181beacc566262743528d5ff9f7d2
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 100%

---

# Fluxo de trabalho de contribuição do GitHub para grandes alterações

<!--
>[!IMPORTANT]
>All repositories that publish to docs.adobe.com have adopted the [Adobe Open Source Code of Conduct](../../code-of-conduct.md) or the [.NET Foundation Code of Conduct](https://dotnetfoundation.org/code-of-conduct). For more information, see the [Contributing](../../contributing.md) article.
>
> Minor corrections or clarifications to documentation and code examples in public repositories are covered by the [Adobe Documentation Terms of Use](https://www.adobe.com/legal/terms.html). New or significant changes generate a comment in the pull request, asking you to submit an online Contribution License Agreement (CLA) if you are not an employee of Adobe. We need you to complete the online form before we can review or accept your pull request.
--->

## Visão geral

Esse fluxo de trabalho é adequado para um colaborador que precisa fazer uma grande alteração ou que será um colaborador frequente de um repositório. Os contribuidores frequentes normalmente fazem alterações contínuas (execução demorada), que passam por vários ciclos de compilação/validação/produção ou que demandam vários dias antes de terem suas solicitações de pull aprovadas e mescladas.

### Terminologia

Antes de começar, vamos rever alguns dos termos do Git/GitHub usados neste fluxo de trabalho.

| Nome | Descrição |
|-----------|-------------|
| bifurcação | Normalmente usado como um substantivo ao se referir a uma cópia de um repositório GitHub principal. Na prática, uma bifurcação é apenas outro repositório. Mas é especial, uma vez que o GitHub mantém uma conexão bidirecional com o repositório principal/pai. Às vezes, é usado como verbo, como em &quot;Você deve bifurcar o repositório primeiro&quot;. |
| remoto | Uma conexão nomeada com um repositório remoto, como o repositório remoto de &quot;origem&quot; ou &quot;upstream&quot;. O Git refere-se a esses repositórios como remotos, pois são usados para fazer referência a um repositório hospedado em outro computador. Nesse fluxo de trabalho, um repositório remoto sempre é um repositório GitHub. |
| origem | O nome atribuído à conexão entre o repositório local e o repositório do qual ele foi clonado. Nesse fluxo de trabalho, a origem representa a conexão com a bifurcação. Às vezes, ela é usada como um moniker do próprio repositório de origem, como em &quot;Lembre-se de enviar as alterações para a origem&quot;. |
| upstream | Assim como o repositório remoto de origem, o repositório upstream é uma conexão nomeada com outro repositório. Nesse fluxo de trabalho, o repositório upstream representa a conexão entre o repositório local e o repositório principal, do qual a bifurcação foi criada. Às vezes, é usado como um moniker para o próprio repositório upstream, como em &quot;Lembre-se de extrair as alterações do upstream&quot;. |

Se você não estiver familiarizado com os conceitos do Git e do GitHub, como um repositório ou ramificação, revise primeiro os [fundamentos de Git e GitHub](git-fundamentals.md).

## Fluxo de trabalho

>[!IMPORTANT]
>
> Se você ainda não tiver feito isso, conclua as etapas na seção [Configuração](github-signup.md).

Nesse fluxo de trabalho, as alterações fluem em um ciclo repetitivo. Começando pelo repositório local do seu dispositivo, elas fluem para a sua bifurcação do GitHub, para o repositório GitHub principal e retornam localmente à medida que você incorpora as alterações de outros colaboradores.

### Usar o fluxo do GitHub

Lembre-se que os [fundamentos do Git e GitHub](git-fundamentals.md) informam que um repositório Git contém uma ramificação principal e outras ramificações de trabalho em andamento adicionais que ainda não foram integradas à ramificação principal. Sempre que você introduz um conjunto de alterações logicamente relacionadas, é recomendável criar uma *ramificação de trabalho* para gerenciar as alterações no fluxo de trabalho. Aqui, nos referimos a isso como uma ramificação de trabalho, porque esse é um espaço de trabalho para iterar/refinar as alterações até que elas possam ser reintegradas na ramificação principal.

Ao isolar as alterações relacionadas em uma ramificação específica, é possível controlar e introduzir as alterações de maneira independente, direcionando-as para um momento de lançamento específico no ciclo de publicação. Na verdade, dependendo do tipo de trabalho, você pode ter várias ramificações funcionais no seu repositório. Não é incomum trabalhar em várias ramificações ao mesmo tempo, cada uma representando um projeto diferente.

>[!NOTE]
>
>Fazer as alterações diretamente na ramificação principal *não é uma prática recomendada*. Imagine que você use a ramificação principal para inserir um conjunto de alterações em uma versão de recurso programada. Você conclui as alterações e aguarda a liberação delas. Logo em seguida, você recebe uma solicitação urgente para corrigir algo; então, você faz a alteração em um arquivo na ramificação principal e a publica. Neste exemplo, você publica inadvertidamente a correção *e* as alterações que estavam aguardando liberação em uma data específica.

A próxima etapa é criar uma nova ramificação de trabalho no repositório local para capturar as alterações propostas. Cada cliente Git é diferente. Consulte a ajuda do seu cliente preferido. Você pode ver uma visão geral do processo no Guia do GitHub no [fluxo do GitHub](https://guides.github.com/introduction/flow/).

## Processamento de solicitação de pull

Você envia as alterações propostas agrupando-as em uma nova solicitação de pull (PR) que é adicionada à fila de PRs do repositório de destino. As solicitações de pull possibilitam o modelo de colaboração do GitHub, solicitando que as alterações feitas em sua ramificação de trabalho sejam extraídas e mescladas com outra ramificação. Na maioria dos casos, essa outra ramificação é a ramificação padrão/principal no repositório principal.

### Validação

Antes da solicitação de pull ser mesclada à ramificação de destino, pode ser necessário passar por um ou mais processos de validação de PR. Os processos de validação podem variar dependendo do escopo das alterações propostas e das regras do repositório de destino. Depois de enviar a solicitação de pull, o conteúdo é revisado e, se e quando apropriado, mesclado com o repositório principal.

### Revisão e aprovação

Após concluir todo o processamento da PR, você deve revisar os resultados (comentários da PR, URLs de visualização, etc.) para determinar se são necessárias alterações adicionais nos arquivos antes de aprovar a mesclagem. Se um revisor de PR tiver revisado sua solicitação de pull, ele também poderá fornecer feedback em comentários, se houver problemas/perguntas pendentes que precisam ser resolvidos antes da mesclagem.

Quando a solicitação de pull estiver livre de problemas e for aprovada, as alterações serão mescladas com a ramificação principal e a solicitação de pull será encerrada.

### Publicação

Lembre-se de que sua solicitação de pull deve ser mesclada por um revisor de PR antes que as alterações possam ser incluídas na próxima execução de publicação programada. As solicitações de pull são normalmente revisadas/mescladas na ordem de envio. Se sua solicitação de pull exigir mesclagem em uma execução de publicação específica, você precisará trabalhar com o revisor de PR antecipadamente para garantir que a mesclagem ocorra antes da publicação.
