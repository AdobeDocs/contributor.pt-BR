---
lastModified: 2018-06-28T00:00:00Z
title: Diretrizes de estilo de criação para colaboradores externos
description: Saiba mais sobre a criação e as diretrizes editoriais para colaboradores externos do Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: tm+mt
source-wordcount: '2227'
ht-degree: 8%

---

# Diretrizes de estilo de criação para colaboradores externos{#guidelines}

Esta página fornece diretrizes editoriais para autores externos que criam conteúdo ou atualizam conteúdo existente no Experience League. Antes de começar, verifique se:

* Familiarize-se com [Markdown](markdown.md) criação
* Verifique a ortografia e a gramática nos artigos
* Use um tom amigável, uma apresentação consistente e frases simples para melhorar a tradução automática
* Seguir [práticas recomendadas](#writing-tips) e padrões editoriais nesta página

## Diretrizes de estilo{#style-guidelines}

Lembre-se do seguinte ao escrever uma documentação:

* **Escreva de maneira concisa**: não desperdice palavras. Mantenha as frases curtas e concisas. Mantenha o foco do artigo. Reduza o número de notas.
* **Concentre-se no público-alvo e na finalidade**: antes de começar a escrever, determine claramente quem é o cliente e qual é a tarefa ele está tentando realizar. Escreva seu artigo para ajudar o cliente a executar essa tarefa.
* **Use exemplos**: forneça exemplos para explicar os conceitos.
* **Organize o conteúdo**: crie seções para dividir as instruções em grupos de etapas mais controláveis. Use uma captura de tela para esclarecer pontos.

## Práticas recomendadas de escrita técnica{#writing-tips}

A escrita técnica, especialmente para a documentação de software, é um setor especializado. Até mesmo o romancista mais prolífico fica atordoado ao tentar escrever técnicas — não porque o material seja complexo ou técnico, mas porque não é fácil fazer informações complexas e técnicas _simples_. Para ter sucesso, seu conteúdo deve ser estruturalmente consistente, digitalizável, reutilizável e fluir pelo pipeline de publicação sem erros de estrutura e sintaxe.

As seções a seguir descrevem problemas comuns que os novos autores devem observar:

### Cabeçalhos não separados por texto (cabeçalhos duplos){#double-headings}

Se você tiver dois cabeçalhos sem texto os separando, adicione texto ausente (para introduzir o segundo cabeçalho de tópico). Ou você pode remover um dos cabeçalhos. A segunda é provavelmente desnecessária.

Por exemplo, _Visão geral_ não serve qualquer objetivo aqui:

![Cabeçalhos duplos](assets/headings-double.png)

* Além disso, se o segundo cabeçalho for _Visão geral_, provavelmente é desnecessário. Seu H1 e o primeiro parágrafo servem como a visão geral conceitual sobre o tópico do artigo.

* Da mesma forma, para fins de SEO, cabeçalhos autônomos como _Visão geral_ e _Introdução_ não são úteis por si só. Dê um nome ao produto ou recurso que você está apresentando. (Exemplo: _Visão geral dos relatórios de Fallout_)

### Cabeçalhos de referência cruzada inconsistentes{#maps}

Use _Mais informações_ títulos para listas de referência cruzada (ou mapas). Exemplo:

![Lista de referências cruzadas](assets/headings-more-info.png)

**Orientações para as listas de referência cruzada**

* Usar uma lista de marcadores para as referências cruzadas
* Use itálico para os nomes formais dos guias ou nomes de página (quando não estiver usando o texto do link)
* Não pontuar o cabeçalho (ou qualquer título)
* Evite números em cabeçalhos

### Entrada de TOC incompatível, navegação estrutural e nome de página{#toc}

Como gerenciamos manualmente o arquivo TOC (índice), essas incompatibilidades são erros fáceis. Certifique-se de que a entrada TOC corresponda ao nome da página (H1). Além disso, certifique-se de que ele esteja perto da navegação estrutural.

**Orientação sobre os sumários e listas**

* Talvez seja necessário encurtar a entrada do TOC, mas ela deve claramente estar relacionada ao nome e à navegação estrutural da página.
* As navegações estruturais são extraídas dos metadados do título, de modo que podem ser diferentes (para fins de SEO).

### Aspas em vez de itálico{#quotes}

É difícil resistir a adicionar aspas em torno de uma palavra ou frase. No entanto, as aspas são destinadas a citar a fala e quase nunca são usadas na documentação do produto.

**Orientação sobre aspas**

* Normalmente, o itálico funciona melhor do que aspas (para mensagens de erro, palavras exclusivas ou estrangeiras e assim por diante).
* Para elementos de interface, use negrito e UICONTROL.

### Procedimentos{#steps}

Escrevendo um procedimento (a variável _tarefa_ tipo de conteúdo) não é um talento com o qual nascemos. A criação de um procedimento legível e claro é uma prática.

**Orientação para etapas**

* Um procedimento é uma série de etapas. Um passo é breve, numerado, _frase única_ comando.
* Inicie cada etapa com um verbo ou o _Para_ infinito (para orientar o leitor para a meta, como em, _Para permanecer conectado, habilite **Permanecer conectado**_). Se uma etapa tiver um objetivo específico no procedimento geral, mencione o objetivo antes da ação.
* Se você tiver informações sobre a etapa (um tipo de conteúdo chamado _informações da etapa_, adicione-o depois da etapa (recuado com a etapa) ou depois do ativo (uma captura de tela, vídeo ou uma lista de descrições da interface).
* Se a sua etapa tiver duas ações (como _Selecione isso e depois_), escreva-a como uma frase simples e breve.
* Limite sua tarefa a cerca de sete a dez etapas. Se você estiver criando mais de dez etapas em uma tarefa, provavelmente precisará dividi-la em duas tarefas. Use seu melhor julgamento aqui.
* Na documentação do produto, não use cabeçalhos como etapas. (Exceção abaixo para tutoriais.)
* Para tutoriais de várias páginas, os cabeçalhos como etapas podem ser permitidos. No entanto, não os numere. Em vez disso, soletrar _Etapa 1:_, _Etapa 2:_ e assim por diante.

**Exemplo de procedimento**

Este é um procedimento bem estruturado para entrar no Adobe:

Para entrar no Adobe:

1. Ligado `Adobe.com`, selecione **Experience Cloud**.
1. Selecionar **Fazer logon**.
1. Selecionar **Conta pessoal**.
1. Para continuar conectado, selecione **Manter sessão iniciada**.
1. Digite seu nome e senha.
1. Selecionar **Fazer logon**.

### Listas paralelas{#lists}

O uso da construção paralela para listas facilita a leitura e a digitalização. As listas incluem um sumário (índice), listas com marcadores (não ordenadas) ou listas numeradas.

Exemplo de índice com entradas paralelas:

![Índice paralelo](assets/parallel-toc.png)

O sumário anterior é um bom exemplo porque:

* As entradas pai conceituais são substantivos ou frases substantivas
* Os procedimentos (tarefas) são verbos ativos (não gerols)
* Todas as entradas usam capitalização da frase

## Metadados de título e descrição{#metadata}

_Título_ e _descrição_ os metadados são importantes para SEO, descoberta de conteúdo e pontuações de qualidade de conteúdo no Experience League.

Veja exemplos de títulos e descrições:

**Descrições de artigos de conceito**

* _Saiba mais sobre segmentos no Adobe Analytics. Obtenha ajuda sobre como configurar o painel Segmentação em um espaço de trabalho._
* _Encontre ajuda sobre como usar segmentos em um relatório de Exibições de página no Adobe Analytics._

**Descrições de artigos de procedimentos/tarefas**

* _Saiba como criar um segmento no Adobe Analytics._
* _Crie um segmento no Adobe Analytics. Saiba como selecionar, configurar e executar um relatório com base no segmento que você cria._

A opção usada depende do tamanho e do escopo do artigo.

**Título de um artigo de conceito**

* _Segmentos nos relatórios de Exibições de página_

**Título de um artigo de procedimento/tarefa**

* _Criar um segmento para um relatório de Exibições de página_

(Lembre-se, o pipe e o nome do produto são adicionados automaticamente aos títulos.)

## Maneiras de melhorar a clareza (e pontuações do Acrolinx){#tips}

Estas são formas simples de melhorar o design do conteúdo, a clareza e a legibilidade. Isso também ajuda a melhorar as pontuações de estilo do Acrolinx e as pontuações do CQI no ExL.

| Orientação | Sobre o  |
|---|---|
| Usar voz ativa | Alterar voz passiva para voz ativa |
| Usar tensão presente | **Fraco:** *O Campaign v8 será lançado em junho.* <p>**Forte:** *Versões v8 do Campaign em junho.*<p>A tensão atual é sempre mais fácil de ler para os clientes. |
| Evite anúncios fracos, inúteis | *Muito raros*, *extremamente*, *incrivelmente*.... <p>Os anúncios são palavras extras que não acrescentam significados significativos se você usar verbos, cláusulas e adjetivos fortes e precisos. |
| Use verbos fortes para títulos e [Entradas de sumário](#using-toc) | Exemplos:<p>**Fraco:** *Criação e gerenciamento de características* <p>**Forte:** *Criar e gerenciar características* |
| Usar frase [capitalização](https://docs.microsoft.com/en-us/style-guide/capitalization) | Na dúvida, não capitalize. Em cabeçalhos, use a capitalização com estilo de frase. Capitalize os nomes próprios e a primeira palavra após dois pontos. Em procedimentos, corresponda à capitalização que você vê na interface. |
| Aprenda estas pequenas dicas para maior clareza | <ul><li>Evitar *Para* (não acrescenta significado). Tudo que você precisa é *a.*</li><li>Evitar *Utilize.* Pode parecer mais técnico, mas não é. *Utilizar* meios *para aproveitar, em especial, algo que não se destinava ao objetivo, mas que servirá*.</li><li>Evite ponto e vírgula: Em vez disso, use ponto e comece uma nova frase. Ponto e vírgula apresenta complexidade desnecessária.</li><li>Dois pontos: Use dois pontos para introduzir uma lista. Use dois pontos com moderação em frases. Capitalize a primeira palavra após dois pontos em uma frase.</li><li>Use a vírgula de Oxford (três vírgulas em uma lista).</li><li>Mantenha a duração da frase abaixo de 39 palavras.</li><li>Navegação: use _ir para_ ou _navegue até_.</li><li>Evite um texto de URL bruto (use um texto de link simples), a menos que a exibição do caminho seja uma informação importante.</li></ul> |
| Usar um verificador ortográfico no VSC | Instale a verificação ortográfica do código (extensão) no Código do Visual Studio. |
| Alterar _click_ para _ir para_ ou _select_ | _Clique em_ é uma palavra específica do dispositivo (com problemas de acessibilidade), e a tendência é se afastar dela. Estas são as sugestões para alterá-la:<ul><li>Navegação: _Vá para Arquivo > Imprimir_.</li><li>Clicando em: _Selecione Arquivo > Imprimir_ ou _Selecione OK_. </li></ul>Consulte [Descrição das interações com a interface do usuário](https://docs.microsoft.com/en-us/style-guide/procedures-instructions/describing-interactions-with-ui) para obter mais ideias sobre a melhor escolha de palavra em várias situações. |
| Execute Acrolinx no VSC | O Acrolinx verifica problemas de estilo e gramática. Verifica URLs, terminologia, ortografia e muito mais. Ajuda a melhorar a clareza e a tradução no conteúdo do Experience League. |

{style=&quot;table-layout:auto&quot;}

Mais algumas práticas recomendadas e recursos:

* [Conteúdo verificável](https://docs.microsoft.com/en-us/style-guide/scannable-content/): Ajude os leitores a encontrar o que precisam rapidamente, ou a reconhecê-lo tão rapidamente quanto quando não estão onde precisam estar. Escrever para facilitar a digitalização pode ajudar.
* **Números:** No texto do corpo, especifique números inteiros de zero a nove e use números para 10 ou maior. Consulte [Números](https://docs.microsoft.com/en-us/style-guide/numbers).
* Escreva como se falasse, projete a amabilidade e chegue rápido ao ponto.

Consulte [As 10 principais dicas de gravação](https://docs.microsoft.com/en-us/style-guide/top-10-tips-style-voice) no [Guia de estilo Microsoft®](https://docs.microsoft.com/en-us/style-guide/welcome/) para obter mais informações.

## Texto alternativo{#alt-text}

Adicione um texto alternativo significativo aos seus ativos (imagens). Considere o texto alternativo que corresponde a:

* A meta que os clientes podem alcançar (nome da tarefa ou do conceito)
* O recurso ou página que você está mostrando
* O nome do ícone que você está mostrando

O Google considera o texto alternativo em resultados de SEO.

## Localização - DNL e UICONTROL{#localization}

Você não precisa se preocupar se o seu produto está localizado ou os idiomas que o ExL usa. No entanto, você ajuda a melhorar a qualidade da localização ao aplicar as duas tags (obrigatórias) do Markdown a seguir, quando apropriado:

* `DNL`

   DNL significa _não traduzir_. Use-o somente para nomes de produtos Adobe de marcas registradas, todos em inglês.

   Exemplos de sintaxe: `[!DNL Adobe Campaign]` ou `[!DNL Workfront]`

   O DNL não se destina a nomes de arquivos ou URLs.

* `UICONTROL`

   UICONTROL indica um controle de interface (como uma opção, campo, guia, página, grupo de opções ou nome do recurso na interface do usuário).

   Exemplo de sintaxe: `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>Você deve aplicar essas tags antes de localizar seu conteúdo.

### Uso do Adobe em nomes de produtos{#product-names}

Para a identidade corporativa, geralmente incluímos _Adobe_ na primeira referência de um produto no nível de guia. Dependendo de considerações de espaço, é possível soltar Adobe em um cabeçalho, mas a primeira referência na cópia de corpo deve incluir o nome completo. Certos produtos, como _Adobe Audition_ e _Adobe Premiere Pro_, exigir a utilização de Adobe em primeira ou mais referência em todas as peças de garantia por fazer parte do nome legal, de marca comercial.

## Primeiro parágrafo{#firstparas}

Seu primeiro parágrafo deve definir o tópico e descrever o que o leitor aprende ao ler o artigo.

Primeiro parágrafo de exemplo (conceito):

_Os públicos-alvo são coleções de visitantes (uma lista de IDs de visitante). A conversão do serviço de público-alvo gerencia os dados do visitante em segmentação do público-alvo. Assim, criar e gerenciar públicos-alvo é como criar e usar segmentos, com a capacidade adicional de compartilhar o segmento do público-alvo com a Experience Cloud._

Primeiro parágrafo de exemplo (tarefa):

_Crie a fonte de atributos do cliente (arquivos CSV e FIN) e faça upload dos dados. É possível ativar a fonte de dados quando você estiver preparado. Quando a fonte de dados estiver ativa, compartilhe os dados de atributo no Analytics e no Target._

### Dicas de SEO para os primeiros parágrafos{#seo}

* Incluir termos de pesquisa nos primeiros parágrafos.
* Use os termos que os leitores usam.
* Inclua sinônimos e, se necessário, o uso anterior dos termos. Por exemplo, &quot;O serviço de Experience Cloud ID (ECID), anteriormente conhecido como _ID de visitante_ ou como acrônimos como MID, MCVID, fornece uma ID persistente e universal que identifica visitantes.&quot;
* Inclua termos de SEO em links.
* Evite colocar termos essenciais em tabelas complexas. Tabelas complexas não produzem resultados de pesquisa confiáveis. O texto em imagens não é pesquisa. As legendas são pesquisadas.

## Capitalização{#capitalization}

* O estilo Adobe usa a capitalização com estilo de frase para todos os títulos, cabeçalhos, subposições e elementos de navegação da página.
* Todas as palavras são minúsculas, exceto a primeira palavra e os nomes próprios, como os nomes de marcas, soluções e serviços.
* Corresponda a capitalização nos nomes de produtos de ferramentas, opções, itens de menu, caixas de diálogo e campos.

## Índice{#using-toc}

O `TOC.md` é seu índice. Cada guia deve ter um.

**Orientação editorial para um sumário**

* Capitalização: Sempre use letras maiúsculas e minúsculas em cada entrada (sem incluir acrônimos). Capitalize somente nomes de produtos formais ou elementos de interface (páginas, guias, campos, opções e assim por diante). Corresponda a interface do usuário ao fazer referência a ela.
* Forma verbal e paralelismo: Use verbo imperativo e evite os fundos. Os TOCs são listas, portanto, sempre tente manter listas paralelas a maior parte do tempo. Há exceções que às vezes não podem ser evitadas. Para páginas conceituais, use substantivos e frases substantivas. Para tarefas, use verbos.

**Orientação de sintaxe**

* Um cabeçalho de seção (pai) no TOC não pode ser um link; ela não tem uma página com conteúdo. Ele deve conter uma âncora como `{#processing-rules}`.
* Você deve usar a sintaxe apropriada para os cabeçalhos da seção TOC (por exemplo, `+ Processing rules {#processing-rules}`) e links de artigos de sumário (por exemplo, `+ [Article name](article.md)`).
* As entradas de artigo de sumário podem ser uma versão reduzida do título do artigo. Siga os padrões para escrever visões gerais, conceitos e tarefas neste documento.
* Evite adicionar o mesmo arquivo várias vezes a um TOC (ou a vários TOCs). Isso causa um comportamento estranho.
* Se o acordo de recompra contiver vários guias do usuário, os diretórios do guia do usuário deverão estar no mesmo nível, como os subdiretórios dentro da variável `help` diretório. Cada diretório do guia do usuário deve ter um arquivo TOC. Nenhum guia de usuário aninhado.

## Negrito e itálico{#bold}

* Use o texto em negrito somente para elementos de interface em um procedimento (e com UICONTROL).
* Use itálico para ênfase ou quando uma palavra é confusa sem ela. Por exemplo, uma palavra estrangeira, ou quando você está descrevendo uma palavra ou definindo um termo.
