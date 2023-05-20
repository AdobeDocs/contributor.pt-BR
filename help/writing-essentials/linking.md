---
lastModified: 2018-06-28T00:00:00Z
title: Uso de links na documentação
seo-title: Using links in Adobe Git/Markdown documentation
description: Este artigo fornece orientação sobre como criar links para conteúdos e imagens.
seo-description: This article provides guidance on creating links to content and images for Adobe documentation.
exl-id: f9d61aa9-931c-4654-ab21-c6e47936954e
source-git-commit: dad1df81797e6078645449501ed0661cf4bcf3ce
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 100%

---

# Uso de links na documentação

Este artigo descreve o uso de hiperlinks nas páginas de documentação. É fácil adicionar links ao Markdown com algumas convenções variáveis. Os links direcionam os usuários para o conteúdo na mesma página, para outras páginas vizinhas ou para sites e URLs externos.

>[!IMPORTANT]
>Todos os links devem ser protegidos (`https` vs. `http`) sempre que o destino permitir (e a grande maioria permite).

## Link a URLs

As palavras que você incluir no texto do link devem ser o título da página que está sendo vinculada ou a um texto específico e descritivo.

**Exemplos:**

- `For more information, see the [overview article](https://github.com/AdobeDocs/target.en/help/overview.md).`

- `For more details, see [Adobe Legal Concerns](https://www.adobe.com/legal).`

## Link de um artigo para outro

Para criar um link em linha de um artigo para outro artigo no mesmo repositório, use a seguinte sintaxe de link:

- Um artigo em um diretório vinculado a outro artigo no mesmo diretório:

   `[link text](article-name.md)`

- Um artigo vinculado de um subdiretório a um artigo no diretório raiz:

   `[link text](../article-name.md)`

- Um artigo vinculado de um subdiretório a um artigo no diretório raiz:

   `[link text](../../article-name.md)`

- Um artigo no diretório raiz vinculado a um artigo em um subdiretório:

   `[link text](./directory/article-name.md)`

- Um artigo em um subdiretório vinculado a um artigo em outro subdiretório:

   `[link text](../directory/article-name.md)`

- Um artigo em um subdiretório vinculado a um artigo em outro subdiretório:

   `[link text](../../directory/article-name.md)`

## Link a âncoras

Não é necessário criar âncoras. Elas são geradas automaticamente no momento da publicação para todos os cabeçalhos H2. A única coisa que você precisa fazer é criar links para as seções H2 (##).

- Para vincular a um cabeçalho no mesmo artigo:

   `[link](#the-text-of-the-level2-section-separated-by-hyphens)`

   `[Link to anchors](#links-to-anchors)`

- Para vincular a uma âncora em outro artigo no mesmo subdiretório:

   `[link text](article-name.md#anchor-name)`

   `[Configure your profile](overview.md#getting-started)`

- Para vincular a uma âncora em outro subdiretório de serviço:

   `[link text](../directory/article-name.md#anchor-name)`

   `[Configure your profile](../overview.md#configure-your-profile)`

## Link a imagens

Como prática recomendada, imagens e arquivos são armazenados em um diretório `assets` no mesmo nível que o arquivo Markdown vinculado a eles.

- Um artigo é vinculado a uma imagem no subdiretório `assets`:

   `![alt text](assets/image-name.png)`

- Um artigo é vinculado a uma imagem no subdiretório `assets/no-localize`:

   `![alt text](assets/no-localize/image-name.png)`
