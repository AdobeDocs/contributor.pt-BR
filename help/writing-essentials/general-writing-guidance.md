---
lastModified: 2018-06-28T00:00:00Z
title: Diretrizes de estilo de criação para colaboradores externos
description: Saiba mais sobre a criação e as diretrizes editoriais para colaboradores externos da Experience League.
exl-id: 874f88d7-18ad-4ac8-bfa3-737255652bbc
source-git-commit: 03d46c9ffb664824f9526f781d776069d486f271
workflow-type: tm+mt
source-wordcount: '2224'
ht-degree: 100%

---

# Diretrizes de estilo de criação para colaboradores externos {#guidelines}

Esta página fornece diretrizes editoriais para autores externos que criam conteúdo ou atualizam conteúdo existente na Experience League. Antes de começar, assegure-se de:

* Estar familiarizado com criação no [Markdown](markdown.md)
* Verificar a ortografia e a gramática nos artigos
* Usar um tom amigável, uma apresentação consistente e frases simples para melhorar a tradução automática
* Seguir as [práticas recomendadas](#writing-tips) e os padrões editoriais nesta página

## Diretrizes de estilo {#style-guidelines}

Lembre-se do seguinte ao escrever uma documentação:

* **Escreva de maneira concisa**: não desperdice palavras. Mantenha as frases curtas e concisas. Mantenha o foco do artigo. Reduza o número de notas.
* **Concentre-se no público-alvo e na finalidade**: antes de começar a escrever, determine claramente quem é o cliente e qual é a tarefa ele está tentando realizar. Escreva seu artigo para ajudar o cliente a executar essa tarefa.
* **Use exemplos**: forneça exemplos para explicar os conceitos.
* **Organize o conteúdo**: crie seções para dividir as instruções em grupos de etapas mais controláveis. Use uma captura de tela para esclarecer pontos.

## Práticas recomendadas de escrita técnica {#writing-tips}

A escrita técnica, especialmente para a documentação de software, é um setor especializado. Até mesmo o romancista mais prolífico fica nervoso ao tentar escrever materiais técnicos, não porque o material é complexo ou técnico, mas porque não é fácil _simplificar_ informações complexas e técnicas. Para ter sucesso, seu conteúdo deve ser estruturalmente consistente, digitalizável, reutilizável e fluir pelo pipeline de publicação sem erros de estrutura e sintaxe.

As seções a seguir descrevem problemas comuns que os novos escritores devem observar:

### Cabeçalhos não separados por texto (cabeçalhos duplos) {#double-headings}

Se você tiver dois cabeçalhos sem texto os separando, adicione o texto ausente (para introduzir o cabeçalho do segundo tópico). Ou você pode remover um dos cabeçalhos. O segundo é provavelmente desnecessário.

Por exemplo, _Visão geral_ não serve qualquer objetivo aqui:

![Cabeçalhos duplos](assets/headings-double.png)

* Além disso, se o segundo cabeçalho for _Visão geral_, ele provavelmente é desnecessário. Seu H1 e o primeiro parágrafo já servem como a visão geral conceitual sobre o tópico do artigo.

* Da mesma forma, para fins de SEO, cabeçalhos autônomos como _Visão geral_ e _Introdução_ não são úteis por si só. Dê um nome ao produto ou recurso que você está apresentando. (Exemplo: _Visão geral dos relatórios de fallout_)

### Cabeçalhos de referência cruzada inconsistentes {#maps}

Use o cabeçalho _Mais informações_ para as listas de referência cruzada (ou mapas). Exemplo:

![Lista de referências cruzadas](assets/headings-more-info.png)

**Orientações para as listas de referência cruzada**

* Use uma lista com marcadores para as referências cruzadas
* Use itálico para os nomes formais dos guias ou nomes de página (quando não estiver usando o texto do link)
* Não pontue o cabeçalho (ou qualquer cabeçalho)
* Evite usar números nos cabeçalhos

### Entrada de índice errada, navegação estrutural e nome de página {#toc}

Como gerenciamos manualmente o arquivo de índice, esses erros são comuns. Certifique-se de que a entrada do índice corresponda ao nome da página (H1). Além disso, certifique-se de que ele corresponda à navegação estrutural.

**Orientação sobre sumários e listas**

* Talvez seja necessário encurtar a entrada do sumário, mas ela deve claramente estar relacionada ao nome e à navegação estrutural da página.
* As navegações estruturais são extraídas dos metadados do título, de modo que podem ser diferentes (para fins de SEO).

### Aspas em vez de itálico {#quotes}

É difícil resistir a adicionar aspas em torno de uma palavra ou frase. No entanto, as aspas são destinadas a citar falas e quase nunca são usadas em documentações de produtos.

**Orientação sobre aspas**

* Normalmente, o itálico funciona melhor do que as aspas (para mensagens de erro, palavras exclusivas ou estrangeiras e assim por diante).
* Para elementos da interface, use negrito e UICONTROL.

### Procedimentos {#steps}

Escrever um procedimento (do tipo de conteúdo _tarefa_) não é um talento nato nosso. Criar um procedimento legível e claro exige prática.

**Orientação para etapas**

* Um procedimento é uma série de etapas. Uma etapa é um comando breve, numerado, de _frase única_.
* Inicie cada etapa com um verbo ou o com a preposição _Para_ seguida do verbo no infinitivo (para orientar o leitor ao objetivo, como em: _Para permanecer conectado, habilite a opção **Permanecer conectado**_). Se uma etapa tiver um objetivo específico no procedimento geral, mencione o objetivo antes da ação.
* Se você tiver informações sobre a etapa (um tipo de conteúdo chamado de _informações da etapa_), adicione-as depois da etapa (recuadas com a etapa) ou depois do ativo (uma captura de tela, vídeo ou uma lista de descrições da interface).
* Se a sua etapa tiver duas ações (como _Selecione isso e, depois, aquilo_), escreva-a como uma frase simples e breve.
* Limite a sua tarefa em torno de sete a dez etapas. Se você estiver criando mais de dez etapas em uma tarefa, provavelmente precisará dividi-la em duas tarefas. Use o seu bom senso.
* Na documentação do produto, não use cabeçalhos como etapas. (Exceção abaixo para tutoriais.)
* Para tutoriais de várias páginas, os cabeçalhos como etapas podem ser permitidos. No entanto, não os numere. Em vez disso, soletre _Etapa 1:_, _Etapa 2:_ e assim por diante.

**Exemplo de procedimento**

Este é um procedimento bem estruturado para fazer logon na Adobe:

Para fazer logon na Adobe:

1. Em `Adobe.com`, selecione **Experience Cloud**.
1. Selecione **Fazer logon**.
1. Selecione **Conta pessoal**.
1. Para continuar conectado, selecione **Permanecer conectado**.
1. Digite seu nome e senha.
1. Selecione **Fazer logon**.

### Listas paralelas {#lists}

O uso da construção paralela para listas facilita a leitura e a verificação. As listas incluem um sumário, listas com marcadores (não ordenadas) ou listas numeradas.

Exemplo de um sumário com entradas paralelas:

![Sumário paralelo](assets/parallel-toc.png)

O sumário anterior é um bom exemplo porque:

* As entradas principais conceituais são substantivos ou frases substantivas
* Os procedimentos (tarefas) são verbos ativos (não gerúndios)
* Todas as entradas usam a capitalização das frases

## Metadados de títulos e descrições {#metadata}

Os metadados de _títulos_ e _descrições_ são importantes para SEO, descoberta de conteúdos e pontuações de qualidade de conteúdo na Experience League.

Estes são exemplos de títulos e descrições:

**Descrições de artigos de conceito**

* _Saiba mais sobre segmentos no Adobe Analytics. Obtenha ajuda sobre como configurar o painel Segmentação em um espaço de trabalho._
* _Encontre ajuda sobre como usar segmentos em um relatório de Exibições de página no Adobe Analytics._

**Descrições de artigos de procedimentos/tarefas**

* _Saiba como criar um segmento no Adobe Analytics._
* _Crie um segmento no Adobe Analytics. Saiba como selecionar, configurar e executar um relatório com base nos segmentos que você cria._

A opção usada depende do tamanho e do escopo do artigo.

**Título para um artigo de conceito**

* _Segmentos nos relatórios de Visualizações de página_

**Título para um artigo de procedimento/tarefa**

* _Crie um segmento para um relatório de Visualizações de página_

(Lembre-se: o pipe e o nome do produto são adicionados automaticamente aos títulos.)

## Maneiras de melhorar a clareza (e as pontuações do Acrolinx) {#tips}

Estas são formas simples de melhorar o design do conteúdo, a clareza e a legibilidade. Isso também ajuda a melhorar as pontuações de estilo do Acrolinx e as pontuações do CQI no ExL.

| Orientação | Sobre o  |
|---|---|
| Use a voz ativa | Mude a voz passiva para voz ativa |
| Use o tempo presente | **Fraco:** *O Campaign v8 sairá em junho.* <p>**Forte:** *O Campaign v8 sai em junho.*<p>O tempo presente é sempre mais fácil de ler para os clientes. |
| Evite usar advérbios fracos e supérfluos | *Muito*, *extremamente*, *incrivelmente*.... <p>Advérbios são palavras extras que não acrescentam informação significativa se você usar verbos, frases e adjetivos fortes e precisos. |
| Use verbos fortes para títulos e [entradas do índice](#using-toc) | Exemplos:<p>**Fraco:** *Criação e gerenciamento de características* <p>**Forte:** *Crie e gerencie características* |
| Use as [letras maiúsculas](https://docs.microsoft.com/pt-br/style-guide/capitalization) como na norma culta | Na dúvida, não use letras maiúsculas. Em cabeçalhos, use as letras maiúsculas como na norma culta. Use letra maiúscula nos substantivos próprios e na primeira palavra após os dois pontos. Em procedimentos, escreva do mesmo jeito que você vê na interface. |
| Lembre-se destas pequenas dicas para maior clareza | <ul><li>Evite a expressão *com o objetivo de* (não acrescenta significado). Tudo que você precisa é *para.*</li><li>Evitar a palavra *Utilizar.* Pode parecer mais técnico, mas não é. *Utilizar* quer dizer *fazer bom uso, em especial, algo que não se destinava a tarefa, mas que servirá*.</li><li>Evite usar o ponto e vírgula: em vez disso, use o ponto final e comece uma nova frase. Pontos e vírgulas introduzem uma complexidade desnecessária.</li><li>Dois pontos: use dois pontos para introduzir uma lista. Use os dois pontos com moderação em frases. Use letra maiúscula na primeira palavra após os dois pontos em uma frase.</li><li>Use a vírgula de Oxford (três vírgulas em uma lista).</li><li>Mantenha o tamanho da frase abaixo de 39 palavras.</li><li>Navegação: use _ir para_ ou _navegar até_.</li><li>Evite um texto de URL bruto (use um hiperlink simples), a menos que a exibição do endereço seja uma informação importante.</li></ul> |
| Usar um verificador ortográfico no VSC | Instale a verificação ortográfica do código (extensão) no Visual Studio Code. |
| Altere _clique_ para _vá para_ ou _selecione_ | _Clique_ é uma palavra específica de dispositivos (com problemas de acessibilidade), e a tendência é parar de usá-la. Estas são as sugestões para alterá-la:<ul><li>Navegação: _Vá para Arquivo > Imprimir_.</li><li>Clique: _Selecione Arquivo > Imprimir_ ou _Selecione OK_. </li></ul>Consulte [Descrever interações com a interface](https://docs.microsoft.com/pt-br/style-guide/procedures-instructions/describing-interactions-with-ui) para ver mais ideias sobre a melhor escolha de palavras em várias situações. |
| Execute o Acrolinx no VSC | O Acrolinx verifica problemas de estilo e gramática. Ele verifica URLs, terminologia, ortografia e muito mais. Ele ajuda a melhorar a clareza e a tradução em conteúdos da Experience League. |

{style="table-layout:auto"}

Mais algumas práticas recomendadas e recursos:

* [Conteúdo verificável](https://docs.microsoft.com/pt-br/style-guide/scannable-content/): ajude os leitores a encontrar o que precisam rapidamente, ou a perceber rapidamente quando não estão onde precisam estar. Escrever de maneira que facilite a verificação pode ajudar.
* **Números:** no corpo de texto, escreva por extenso números inteiros de zero a nove e use numerais para 10 ou mais. Consulte [Números](https://docs.microsoft.com/pt-br/style-guide/numbers).
* Escreva como você fala, projete simpatia e vá direto ao ponto.

Consulte as [10 principais dicas de escrita](https://docs.microsoft.com/pt-br/style-guide/top-10-tips-style-voice) no [Guia de estilo da Microsoft®](https://docs.microsoft.com/pt-br/style-guide/welcome/) para obter mais informações.

## Texto alternativo {#alt-text}

Adicione textos alternativos relevantes aos seus ativos (imagens). Considere textos alternativos que correspondam:

* Ao objetivo que os clientes podem alcançar (nome da tarefa ou do conceito)
* Ao recurso ou página que você está mostrando
* Ao nome do ícone que você está mostrando

O Google considera o texto alternativo nos resultados de SEO.

## Localização — DNL e UICONTROL {#localization}

Você não precisa se preocupar se o seu produto está localizado ou com os idiomas que o ExL usa. No entanto, você pode ajudar a melhorar a qualidade da localização aplicando as duas tags (obrigatórias) do Markdown a seguir, quando apropriado:

* `DNL`

   DNL significa _não localizar_. Use-a somente para nomes de produtos da Adobe com marcas registradas, pois eles devem permanecer em inglês.

   Exemplos de sintaxe: `[!DNL Adobe Campaign]` ou `[!DNL Workfront]`

   O DNL não se destina a nomes de arquivos ou URLs.

* `UICONTROL`

   A tag UICONTROL indica um controle de interface (como uma opção, campo, guia, página, grupo de opções ou nome de recurso na interface).

   Exemplo de sintaxe: `Select **[!UICONTROL Project]**, then select **[!UICONTROL Save]**.`

>[!IMPORTANT]
>
>Você deve aplicar essas tags antes de localizar seu conteúdo.

### Uso de Adobe em nomes de produtos {#product-names}

Para manter a identidade corporativa, geralmente incluímos _Adobe_ na primeira referência a um produto no nível do guia. Dependendo do espaço, é possível omitir o nome Adobe em um cabeçalho, mas a primeira referência no corpo do texto deve incluir o nome completo. Certos produtos, como _Adobe Audition_ e _Adobe Premiere Pro_, exigem a utilização do nome Adobe na primeira ou na mais proeminente referência em todas as peças colaterais por fazer parte do nome legal e marca comercial.

## Primeiro parágrafo {#firstparas}

Seu primeiro parágrafo deve definir o tópico e descrever o que o leitor aprenderá ao ler o artigo.

Exemplo de primeiro parágrafo (conceito):

_Públicos são coleções de visitantes (uma lista de IDs de visitante). Os serviços de público da Adobe gerenciam a conversão dos dados de visitantes na segmentação de público. Assim, criar e gerenciar públicos é como criar e usar segmentos, com a capacidade adicional de compartilhar o segmento de público com a Experience Cloud._

Exemplo de primeiro parágrafo (tarefa):

_Crie a fonte de atributos do cliente (arquivos CSV e FIN) e faça upload dos dados. É possível ativar a fonte de dados quando você estiver preparado. Quando a fonte de dados estiver ativa, compartilhe os dados de atributo no Analytics e no Target._

### Dicas de SEO para primeiros parágrafos {#seo}

* Incluir termos de pesquisa nos primeiros parágrafos.
* Use os termos que os leitores usam.
* Inclua sinônimos e, se necessário, os termos cujo uso já é obsoleto. Por exemplo: “O serviço Experience Cloud ID (ECID), anteriormente conhecido como _ID de visitante_ ou por abreviações, como MID, MCVID, fornece uma ID persistente e universal que identifica visitantes.”
* Inclua termos de SEO em links.
* Evite colocar termos essenciais em tabelas complexas. Tabelas complexas não produzem resultados de pesquisa confiáveis. O texto em imagens não é pesquisado. As legendas são pesquisadas.

## Uso de letras maiúsculas {#capitalization}

* O estilo da Adobe usa maiúsculas como norma culta para todos os títulos, cabeçalhos, subtítulos e elementos de navegação da página.
* Todas as palavras são escritas em minúscula, exceto a primeira palavra e os substantivos próprios, como os nomes de marcas, soluções e serviços.
* Siga o estilo de uso de maiúsculas nos nomes de ferramentas, opções, itens de menu, caixas de diálogo e campos que o produto usa.

## Índice {#using-toc}

O `TOC.md` é seu índice. Cada guia deve ter um.

**Orientação editorial para um índice**

* Uso de maiúsculas: sempre use as maiúsculas como na norma culta em cada entrada (exceto abreviações). Use letras maiúsculas somente nos nomes de produtos formais ou elementos de interface (páginas, guias, campos, opções e assim por diante). Siga a interface ao fazer referência a ela.
* Forma verbal e paralelismo: use os verbos no modo imperativo e evite gerúndios. Os índices são listas, portanto, sempre tente manter listas paralelas na maior parte do tempo. Há exceções que às vezes não podem ser evitadas. Para páginas conceituais, use substantivos e frases nominais. Para tarefas, use verbos.

**Orientação de sintaxe**

* Um cabeçalho de seção (principal) no índice não pode ser um link. Ele não tem uma página com conteúdo. Ele deve conter uma âncora como `{#processing-rules}`.
* Você deve usar sintaxe normal para os cabeçalhos da seção de índice (por exemplo, `+ Processing rules {#processing-rules}`) e links de artigos do índice (por exemplo, `+ [Article name](article.md)`).
* As entradas de artigo do índice podem ser uma versão reduzida do título do artigo. Siga os padrões para escrever visões gerais, conceitos e tarefas neste documento.
* Evite adicionar o mesmo arquivo várias vezes a um índice (ou a vários índices). Isso causa um comportamento estranho.
* Se o acordo de recompra contiver vários guias do usuário, os diretórios do guia do usuário deverão estar no mesmo nível, como os subdiretórios dentro do diretório `help`. Cada diretório do guia do usuário deve ter um arquivo índice. Nenhum guia de usuário aninhado.

## Negrito e itálico {#bold}

* Use o texto em negrito somente para elementos de interface clicáveis em um procedimento (e com UICONTROL).
* Use itálico para ênfase ou quando uma palavra for confusa. Por exemplo, uma palavra estrangeira, ou quando estiver descrevendo uma palavra ou definindo um termo.
