---
title: Configurar o repositório Git localmente
seo-title: Configurar o repositório Git localmente para a documentação da Adobe
description: Este artigo fornece orientação para criar seu repositório Git local e contribuir com a documentação da Adobe, incluindo o processo de bifurcamento e clonagem.
seo-description: Este artigo fornece orientação para criar seu repositório Git local e contribuir com a documentação da Adobe, incluindo o processo de bifurcamento e clonagem.
translation-type: tm+mt
source-git-commit: e7382ef4aefc69c6b4e7d78b7f34eaf897596eaf

---


# Configurar o repositório Git localmente para a documentação

Este artigo descreve as etapas para configurar um repositório Git no computador local, com o objetivo de contribuir para a documentação da Adobe. Os colaboradores podem usar um repositório clonado localmente para adicionar novos artigos, fazer grandes edições nos artigos existentes ou alterar a arte-final.

> [!IMPORTANT]
> Se você estiver fazendo apenas pequenas alterações em um artigo, *não* será necessário executar as etapas deste artigo. Basta clicar no ícone Edit e fazer as edições de texto no navegador.

## Visão geral

Para contribuir com a documentação da Adobe, você pode bifurcar o repositório apropriado em sua conta GitHub para obter permissões de leitura/gravação. Em seguida, você pode criar e editar os arquivos do Markdown localmente, clonando o repositório correspondente da documentação. Você usa solicitações de pull para mesclar (enviar) alterações no repositório compartilhado central somente leitura.

* Determine o repositório apropriado
* Bifurque o repositório para sua conta GitHub
* Escolha uma pasta local para os arquivos clonados
* Clone o repositório no computador local
* Configure o valor do repositório remoto/upstream

## Determine o repositório

Você bifurca o repositório apropriado em sua própria conta GitHub para obter permissões de leitura/gravação e armazenar as alterações propostas. [!UICONTROL Adobe Experience Cloud] a documentação está em vários repositórios diferentes em [github.com](https://www.github.com/adobedocs).

1. Se não tiver certeza de qual repositório usar, acesse o artigo usando seu navegador da web. Selecione o link **Edit** (ícone de lápis) no canto superior direito do artigo. (Caso não veja um link Edit, o conteúdo ainda não está disponível no GitHub.)

Para contribuir com a documentação da Adobe, é possível criar e editar os arquivos do Markdown localmente, clonando o repositório correspondente da documentação. Você usa solicitações de pull para mesclar alterações no repositório compartilhado central somente leitura.

<!---
![GitHub Triangle](/assets/git-and-github-initial-setup.png)

If you're new to GitHub, watch the following video for a conceptual overview of the forking and cloning process:

>[!VIDEO https://channel9.msdn.com/Blogs/CoolMoose/Git-Repository-Setup/player]
-->

## Bifurque o repositório

Usando o repositório apropriado, crie uma bifurcação do repositório em sua conta GitHub usando o site do GitHub.

Uma bifurcação pessoal é necessária, pois todos os repositórios de documentação principais fornecem acesso somente leitura, o que significa que não é possível fazer alterações diretamente no conteúdo dos repositórios. Para fazer alterações, você deve enviar uma solicitação de pull (PR) a partir da sua bifurcação para o repositório principal. Para facilitar esse processo, primeiro você precisa ter sua própria cópia do repositório, à qual terá acesso de gravação. Uma *bifurcação* do GitHub é usada para esse fim.

1. Vá para a página do repositório GitHub principal e clique no botão **Fork** (Bifurcar) na parte superior direita.

   ![Bifurcação do GitHub](assets/fork-simple.png)

1. Se solicitado, selecione o bloco da sua conta GitHub como destino para criar a bifurcação. Esse prompt cria uma cópia do repositório na sua conta GitHub, conhecida como uma bifurcação.

1. Escolha um nome de pasta fácil de memorizar e digitar.

   Alguns repositórios podem ser grandes. Escolha um local com espaço disponível em disco.

   > [!NOTE]
   > Evite escolher um caminho de pasta local aninhado com outro local de pasta de repositório Git. Embora seja aceitável armazenar as pastas Git clonadas adjacentes entre si, o aninhamento de pastas Git umas dentro das outras causa erros no rastreamento de arquivos.

## Crie um clone local do repositório

Ao criar um clone do repositório bifurcado, você faz download de uma cópia dos arquivos no seu computador. Quando estiver pronto, você pode enviar as edições da sua unidade local para o repositório bifurcado no servidor. Em seguida, você pode enviar uma solicitação de pull para mesclar as edições ao repositório principal.

Essas etapas consideram que você está usando o GitHub Desktop. Se você estiver usando um cliente diferente, faça os ajustes adequados.

1. Clique em **Clone or download** (Clonar ou fazer download) e escolha **Open in Desktop** (Abrir no computador) para extrair uma cópia do repositório (sua bifurcação) no computador no diretório atual.

![Clone o repositório](assets/clone-pulldown.png)

1. Use o GitHub Desktop para manter os arquivos locais sincronizados com o repositório bifurcado.

Para obter detalhes, consulte a [Documentação do GitHub Desktop](https://help.github.com/desktop/).
