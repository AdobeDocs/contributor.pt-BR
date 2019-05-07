---
lastModified: '2018-06-28'
title: Uso de links na documentação
seo-title: Usar links na documentação do Adobe Git/Markdown
description: Este artigo fornece orientação sobre como criar links para conteúdos e imagens.
seo-description: Este artigo fornece orientação sobre como criar links para conteúdos e imagens para a documentação da Adobe.
translation-type: ht
source-git-commit: 9060d24142e0f03283b42a2a4bbc638abe2952aa

---


# Uso de links na documentação

Este artigo descreve o uso de hiperlinks nas páginas de documentação. É fácil adicionar links ao Markdown com algumas convenções variáveis. Os links direcionam os usuários para o conteúdo na mesma página, para outras páginas vizinhas ou para sites e URLs externos.

> [!IMPORTANT]
> Todos os links devem ser protegidos (`https` vs. `http`) sempre que o destino permitir (e a grande maioria permite).

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

<!--
## Bob's link test

<table id="table_C27955F6B52A45B28BEEAAF14FFC86D8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> File Type </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .csv </span> </p> </td> 
   <td colname="col2"> <p>A comma-separated values file (such as one created in Excel). This is the file that contains the customer attribute data. See [Link TEST](/help/setup/full-workflow.md) </p> <p> <b>Naming requirements:</b> Ensure that file name extensions do not contain white spaces. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .fin </span> </p> </td> 
   <td colname="col2"> <p>(Required) The <span class="filepath"> .fin </span> file tells the system that you are finished uploading data. The name of the <span class="filepath"> .fin </span> file must match the name of the <span class="filepath"> .csv </span> file. </p> <p>Adobe recommends creating an empty text file with a <span class="filepath"> .fin </span> extension. An empty file saves space and upload time. </p> <p> <p>Note:  Renaming a <span class="filepath"> .fin </span> file is not allowed after it is uploaded. The <span class="filepath"> .fin </span> file must be uploaded separately and cannot be a renamed, previously uploaded file. </p> </p> <p>After you upload the <span class="filepath"> .fin </span> file in the customer attributes FTP, the system retrieves data quickly (within one minute). This differs from other Adobe FTP-based systems, which pick up data less frequently (around once per hour). </p> <p>The <span class="filepath"> .fin </span> file is not required when using the drag-and-drop upload method. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="filepath"> .gz </span> or <span class="filepath"> .zip </span> </p> </td> 
   <td colname="col2"> <p> <span class="filepath"> .gz </span> (gzip) or <span class="filepath"> .zip </span> - for compressed files. A <span class="filepath"> .zip </span> file cannot contain more than one file in the archive. </p> <p> <b>Naming requirements:</b> The name of the <span class="filepath"> .zip </span> or <span class="filepath"> .gz </span> should match the name of the <span class="filepath"> .csv </span>. For example, if your <span class="filepath"> .csv </span> file is <span class="filepath"> crm_small.csv </span>, the <span class="filepath"> .zip </span> file should be <span class="filepath"> crm_small.csv.zip </span>. </p> <p>The .fin file must match the .csv. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
