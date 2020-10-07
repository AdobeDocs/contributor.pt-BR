---
lastModified: 2018-06-28T00:00:00Z
title: Como usar o Markdown para escrever a documentação
seo-title: Como usar o Markdown para escrever a documentação da Adobe
description: este artigo fornece informações básicas e de referência sobre a linguagem do Markdown usada para escrever artigos.
seo-description: este artigo fornece informações básicas e de referência sobre a linguagem do Markdown usada para escrever artigos para a documentação da Adobe.
translation-type: ht
source-git-commit: 4ebbbde3337183a19fd3a59ae091b621a092e6f8
workflow-type: ht
source-wordcount: '1322'
ht-degree: 100%

---


# Como usar o Markdown para escrever a documentação técnica

Os artigos técnicos da Adobe são escritos em uma linguagem de marcação simples chamada [Markdown](https://daringfireball.net/projects/markdown/), que facilita a leitura e o aprendizado.

Como estamos armazenando o conteúdo dos documentos da Adobe no GitHub, uma versão do Markdown chamada [GitHub Flavored Markdown (GFM)](https://help.github.com/categories/writing-on-github/) pode ser usada, a qual oferece funcionalidade adicional para as necessidades comuns de formatação. Além disso, a Adobe estendeu o Markdown de algumas maneiras para oferecer suporte a determinados recursos relacionados a ajuda, como notas, dicas e vídeos incorporados.

## Noções básicas sobre o Markdown

### Cabeçalhos

Para criar um cabeçalho, use uma marca de hash (#) no início de uma linha:

```
   # This is level 1 (article title)
   ## This is level 2
   ### This is level 3
   #### This is level 4
   ##### This is level 5
```

### Texto básico

Um parágrafo não requer sintaxe especial no Markdown.

Para formatar o texto como **negrito**, coloque-o entre dois asteriscos. Para formatar o texto como *itálico*, coloque-o entre um único asterisco:

```markdown
    This text is **bold**.
    This text is *italic*.
    This text is both ***bold and italic***.
```

<!--
To format superscript (H<sub>2</sub>O) and subscript (e=mc<sup>2</sup>) text:

```markdown
This is subscript H<sub>2</sub>O and superscript e=mc<sup>2</sup>.
```
-->

Para ignorar os caracteres de formatação do Markdown, use \ antes do caractere:

```markdown
This is not \*italicized\* type.
```

### Listas numeradas e listas de itens

Para criar listas numeradas, comece uma linha com `1.` ou `1)`, mas não use ambos os formatos dentro da mesma lista. Você não precisa especificar os números. O GitHub faz isso para você.

```markdown
1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.
```

Exibido:

1. This is step 1.
1. This is the next step.
1. This is yet another step, the third.

<!-- markdownlint-disable MD037 -->
Para criar listas de itens, comece uma linha com \* ou - ou +, mas não misture os formatos em uma mesma lista. (Não misture formatos de marcadores, como \* e \+, dentro do mesmo documento.)
<!-- markdownlint-disable MD037 -->

```markdown
* First item in an unordered list.
* Another item.
* Here we go again.
```

Exibido:

* First item in an unordered list.
* Another item.
* Here we go again.

Também é possível incorporar listas em listas e adicionar conteúdo entre itens de lista.

```markdown
1. Set up your table and code blocks.
1. Perform this step.

   ![screen](assets/no-localize/adobe_standard_logo.png)
1. Make sure that your table looks like this: 

   | Hello | World |
   |---|---|
   | How | are you? |  
1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.

1. Do another step.
```

Exibido:

1. Set up your table and code blocks.
1. Perform this step.

   ![tela](assets/no-localize/adobe_standard_logo.png)
1. Make sure that your table looks like this:

   | Hello | World |
   |---|---|
   | How | are you? |
1. This is the fourth step.

   >[!NOTE]
   >
   >This is note text.

1. Do another step.

### Tabela

As tabelas não fazem parte da especificação principal do Markdown, mas a Adobe oferece suporte a elas até certo ponto. O Markdown não é compatível com listas de várias linhas em células. A prática recomendada é evitar o uso de várias linhas em tabelas. É possível criar tabelas usando a barra vertical (|) para definir colunas e linhas. Os hifens criam o cabeçalho de cada coluna, enquanto que as barras separam cada coluna. Inclua uma linha em branco antes da tabela para que ela seja renderizada corretamente.

```markdown
| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | column 2 | column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |
```

Exibido:

| Header | Another header | Yet another header |
|--- |--- |--- |
| row 1 | column 2 | column 3 |
| row 2 | row 2 column 2 | row 2 column 3 |

Tabelas simples funcionam adequadamente no Markdown. No entanto, as tabelas que incluem vários parágrafos ou listas dentro de uma célula são difíceis de trabalhar. Para tal conteúdo, recomendamos usar um formato diferente, como cabeçalhos e texto.

Para obter mais informações sobre como criar tabelas, consulte:

* [Como organizar informações com tabelas do GitHub](https://help.github.com/articles/organizing-information-with-tables/)
* O aplicativo web [Gerador de tabelas para Markdown](https://www.tablesgenerator.com/markdown_tables)
* [Converter tabelas HTML para Markdown](https://jmalarcon.github.io/markdowntables/)

### Links

A sintaxe do Markdown para um link em linha consiste na parte `[link text]`, que é o texto que será aplicado ao hiperlink, seguida pela parte `(file-name.md)`, que é o URL ou o nome do arquivo ao qual está sendo vinculado:

`[link text](file-name.md)`

```markdown
[Adobe](https://www.adobe.com)
```

Exibido:

[Adobe](https://www.adobe.com)

Para links para artigos (referências cruzadas) no repositório, use links relativos. Você pode usar todos os operandos de links relativos, como ./ (diretório atual), ../ (voltar um diretório) e ../../ (voltar dois diretórios).

```markdown
See [Overview example article](../../overview.md)
```

Para obter mais informações sobre links, consulte o artigo [Links](linking.md) deste guia para obter a sintaxe do link.

### Imagens

```markdown
![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")
```

Exibido:

![Adobe Logo](assets/no-localize/adobe_standard_logo.png "Hover text")

### Blocos de código

O Markdown oferece suporte à adição em linha de blocos de código em uma sentença e como um bloco “cercado” separado entre sentenças. Para obter detalhes, consulte o [suporte nativo do Markdown para blocos de código](https://daringfireball.net/projects/markdown/syntax#precode)

Use acentos graves ( \` ) para criar estilos de código em linha em um parágrafo. Para criar um bloco de código de várias linhas específico, adicione três acentos graves (\`\`\`) antes e depois do bloco de código (chamado de “bloco de código cercado” no Markdown e apenas um componente de &quot;bloco de código&quot; no AEM). Para blocos de código cercados, adicione o texto do código depois do primeiro conjunto de acentos graves para que o Markdown aponte a sintaxe de código correta. Exemplo: \`\`\`javascript

Exemplos:

```markdown
This is `inline code` within a paragraph of text.
```

Exibido:

This is `inline code` within a paragraph of text.

Isso é um bloco de código cercado:

```markdown
\```javascript
function test() {
 console.log("notice the blank line before this function?");
\```
```

Exibido:

```javascript
function test() {
 console.log("notice the blank line before this function?");
```

### Listas de definições

Uma lista de definição é uma extensão do Markdown que é compatível com o componente de Lista de definições no AEM. Uma lista de definições consiste em um termo e sua definição.

<!--

```markdown
Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
```

Displayed:

Frog
: An amphibious green creature. Likes flies.

Cat
: A less amphibious creature than frogs.
--->

#### Observações e comentários

Comentários (observações) não aparecem nos artigos de ajuda voltados ao público. No entanto, os comentários aparecem nos arquivos do Markdown voltados ao público que os usuários podem visualizar e editar.

## Extensões personalizadas do Markdown

Os artigos da Adobe usam o Markdown padrão para a maioria das formatações, como parágrafos, links, listas e cabeçalhos. Para obter uma formatação mais avançada, os artigos podem usar recursos estendidos do Markdown, como:

* Blocos de notas
* Vídeos incorporados
* Não traduzir
* Propriedades de componente, como atribuir uma ID de cabeçalho diferente a um cabeçalho

Use a aspa de bloco ( > ) do Markdown no início de cada linha para unir um componente estendido, como uma nota. Se você precisar usar subcomponentes dentro de componentes, adicione um nível extra de aspas de bloco (>  >) nessa seção de subcomponente. Por exemplo, uma OBSERVAÇÃO em uma seção DONOTLOCALIZE deve começar com >    >.

Alguns elementos comuns do Markdown, como cabeçalhos e blocos de código, incluem propriedades estendidas. Se você precisar alterar as propriedades padrão, adicione os parâmetros em chaves francesas /{ /} depois do componente. As propriedades estendidas estão descritas em contexto.

### Blocos de notas

É possível escolher entre quatro tipos de blocos de notas para chamar a atenção para um conteúdo específico:

* `[!NOTE]`
* `[!CAUTION]`
* `[!TIP]`
* `[!IMPORTANT]`

Em geral, os blocos de notas devem ser usados com moderação, pois podem causar problemas. Embora também sejam compatíveis com blocos de código, imagens, listas e links, tente manter os blocos de notas simples e diretos.


```markdown
>[!NOTE]
>
>This is a standard NOTE block.
```

Exibido:

>[!NOTE]
>
>This is a standard NOTE block.

```markdown
>[!TIP]
>
>This is a standard tip.
```

Exibido:

>[!TIP]
>
>This is a standard tip.

### Vídeos

Os vídeos incorporados não serão renderizados nativamente no Markdown, mas você poderá usar essa extensão do Markdown.

```markdown
>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12)
```

Exibido:

>[!VIDEO](https://video.tv.adobe.com/v/29770/?quality=12&captions=por_br)

### Mais artigos como este

O componente &quot;Mais artigos como este&quot; no AEM aparece no fim de um artigo. Ele exibe links relacionados. Quando o artigo é renderizado, ele pode ser formatado como um cabeçalho de nível 2 (##) sem ser adicionado ao mini-TOC.

```markdown
>[!MORELIKETHIS]
>* [Article 1](https://helpx.adobe.com/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/support/audience-manager.html)
```

Exibido:

>[!MORELIKETHIS]
>* [Article 1](https://helpx.adobe.com/br/support/analytics.html)
>* [Article 2](https://helpx.adobe.com/br/support/audience-manager.html)


### DNL - Não traduzir - e UICONTROL

Em alguns casos, é necessário sinalizar determinadas seções de conteúdo em um artigo como somente em inglês.
Palavras, frases e outros elementos precisam ser declarados para nossos sistemas de tradução e isso permite gerenciar um léxico controlado.

Para palavras ou frases que não devem ser traduzidas, use a extensão do `[!DNL]` para envolver a palavra ou a seção.

Para elementos na interface do usuário e nos menus de uma solução, usamos a extensão do ``.

**Exemplo:**

In [!DNL Adobe Target] you can create your tests directly on a [!DNL Target]-enabled page.

**Fonte:**

```markdown
In [!DNL Adobe Target] you can create your tests directly on a [!DNL Target]-enabled page.
```

**Exemplo**

Use the [!UICONTROL Visual Experience Composer] in [!DNL Target] to create your test directly on a page.

**Fonte:**

```markdown
Use the [!UICONTROL Visual Experience Composer] in [!DNL Target] to create your test directly on a page.
```

## Identificar e solucionar problemas

### Texto alternativo

O texto alternativo que contém sublinhados não será renderizado corretamente. Por exemplo, em vez de usar isso:

```markdown
![Settings_Step_2](/assets/settings_step_2.png)
```

Nossa prática recomendada é usar hifens (-) em vez de sublinhados (_) nos nomes de arquivo.

```markdown
![Settings-Step-2](/assets/settings-step-2.png)
```

### Apóstrofos e aspas

Se você copiar o texto em um editor do Markdown, poderá conter apóstrofos ou aspas &quot;inteligentes&quot; (curvos). Eles precisam ser codificados ou alterados para apóstrofos ou aspas básicos. Caso contrário, você terá caracteres estranhos como este quando o arquivo for publicado: Itâ€™s

Estas são as codificações das versões &quot;inteligentes&quot; dessas marcas de pontuação:

* Aspas à esquerda (abertura): `&#8220;`
* Aspas à direita (fechamento): `&#8221;`
* Aspas simples (fechamento) ou apóstrofe: `&#8217;`
* Aspas simples (abertura) aspas simples (raramente usadas): `&#8216;`

### Colchetes

Se você usar colchetes no texto (não código) no arquivo - por exemplo, para indicar um espaço reservado -, será necessário codificar os colchetes manualmente. Caso contrário, o Markdown os considerará tags HTML.

Por exemplo, codifique `<script name>` como `&lt;script name&gt;`

### “E” comercial em títulos

“E” comercial (&amp;) não é permitido em títulos. Use &quot;e&quot; ou a codificação `&amp;`.

## Consulte também

### Recursos do Markdown

* [Introdução ao Markdown](https://daringfireball.net/projects/markdown/syntax)
* [Fundamentos do Markdown do GitHub](https://help.github.com/articles/markdown-basics/)
