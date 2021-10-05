# Criando widgets na plataforma Android - Revista Mobile Magazine 45

## Este artigo ensina como um desenvolvedor pode fazer uso do conceito de Widgets na plataforma mobile Android.

[Artigos](https://www.devmedia.com.br/artigos/)[Mobile](https://www.devmedia.com.br/artigos/mobile)Criando widgets na plataforma Android - Revista Mobile Magazine 45



***\*De que se trata o artigo\****



Este artigo ensina como um desenvolvedor pode fazer uso do conceito de Widgets na plataforma mobile Android. Com mais esta feature, seu aplicativo permite um acesso rápido as informações mais relevantes de seu produto, causando um maior apego em seu cliente e potencializando suas receitas e formas de atingir o público alvo.

**
\**Em que situação o tema é útil\****

O tema é extremamente importante para desenvolvedores que querem permitir que seu aplicativo forneça acesso rápido a informação com maior potencialidade. Além disso, se bem feito, seu aplicativo ganhará um espaço de destaque no lugar mais valioso dos aparelhos Android, a Home Screen.

**Criando widgets na plataforma Android**

Este artigo apresentará na prática como podemos desenvolver widgets na plataforma Android. Para isso, conheceremos inicialmente o que são widgets e qual sua importância no cenário atual para desenvolvimento de sistemas para dispositivos móveis. Na sequência, será apresentado passo a passo o desenvolvimento de um widget integrado a redes sociais.

**Autores: Ricardo Ogliari e Robison Cris Brito**



Depois da revolução que o mercado mobile sofreu e, consequentemente, os novos rumos que o mercado de aplicativos móveis tomou, os smartphones dos usuários modernos contêm uma variedade muito grande de aplicativos e jogos. Às vezes, esta quantidade muito grande de opções pode deixar de ser algo benéfico e fazer com que seu aplicativo fique perdido na lista gigantesca de instalações de seus clientes.

Porém, como o mercado mobile é conduzido por empresas muito inteligentes e antenadas nos problemas que cercam este mundo, diversas plataformas estão fornecendo uma maneira mais rápida e inteligente para usuários acessarem informações que eles consideram relevantes.

Um bom exemplo pode ser a plataforma Windows Phone. Ela nos trouxe o conceito de Live Tiles. O tile pode ser entendido como ícone da nossa aplicação. Porém, ele permite atualização de conteúdo, seja ele texto ou imagem. E o usuário pode configurar quais live tiles ficarão na sua tela principal e quais ganharão mais destaque. Desta forma, em dada ocasião, onde o mesmo esteja com muita pressa e precise urgentemente de uma informação, ele pode simplesmente olhar para o tile e não precisar entrar no aplicativo.

Porém, o Windows Phone não foi o pioneiro nesta ideia. O Android nos trouxe há muito tempo o conceito de Widgets. Um Widget pode ser entendido como um miniaplicativo, com um espaço menor e com possibilidade de atualização a uma frequência definida pelo usuário. Além disso, ele pode levar a uma versão completa do software. Por exemplo, coma febre das redes sociais, todo mundo gostar de dar uma olhada rápida nas atualizações e ainda ver a previsão do tempo. Se caso precisasse iniciar dois aplicativos para isso, teria que perder um tempo. Porém, ao configurar dois widgets para ficarem na *home screen*, as informações são acessadas instantaneamente. Sendo assim, basta destravar o aparelho e ter acesso às informações desejadas.

Um bom exemplo de widget pode ser encontrado inclusive na própria documentação do Android. Observe na **Figura 1** um widget para tocar mídias.

![img](https://arquivo.devmedia.com.br/REVISTAS/mobile/imagens/45/05_Widgets_Android/image001.gif)

**Figura 1**. Exemplo de widget de aplicativo de mídia.

Porém, podemos citar inúmeros possíveis aplicativos onde este conceito se encaixaria perfeitamente como, aplicativo de ações, redes Sociais e esportes.

Essa lista poderia se estender por mais algumas páginas, porém, acredito que a importância do conceito de widget já esteja presente na vida do leitor, principalmente se o mesmo for um usuário de smartphones. Para conhecermos a arquitetura e a forma de programação deste conceito na plataforma Android, vamos criar um aplicativo que fica mostrando o último tweet postado em em uma rede social, atualizando o conteúdo em um intervalo de dois minutos.

**O Aplicativo**

O aplicativo proposto será um widget que poderia fazer parte de um aplicativo leitor de tweets. Neste caso, o usuário teria sua vida facilitada porque não precisaria procurar na lista de dispositivos instalados, depois iniciar o aplicativo para, só então, ter acesso às atualizações de sua fonte favorita.

A tela de configuração mostrada na **Figura 2** mostra dois campos de texto. Uma para mostrar a fonte de onde buscaremos os tweets e um campo onde podemos inserir qual o intervalo de atualização que queremos.

![img](https://arquivo.devmedia.com.br/REVISTAS/mobile/imagens/45/05_Widgets_Android/image002.png)

**Figura 2**. Tela de configuração.

A parte mais importante de nosso aplicativo é mostrada na **Figura 3**. Nosso widget apresentará a última atualização feita no tweeter que informamos na tela de configuração.

![img](https://arquivo.devmedia.com.br/REVISTAS/mobile/imagens/45/05_Widgets_Android/image003.png)

**Figura 3**. Widget presente na Home Screen.

**Começando a construção**

Para construir um widget, basicamente precisamos ter em mente que teremos três componentes essenciais:

• *AppWidgetProviderInfo*: este é um metadado que descreve as principais características do widget como: seu espaço mínimo em largura e altura, seu tempo de atualização em milissegundos, o layout inicial apresentado na home screen e uma possível tela de configuração;

• *AppWidgetProvider*: uma classe que herdará de AppWidgetProvider. Esta, por sua vez, é filha de BroadcastReceiver. Porém, ela já trata as principais ações recebidas e que necessitam de tratamento. Pense na mesma como um auxílio que já filtra o *onReceive* e repassa para alguns métodos que devem ser sobrescritos.

• *Layout*: também necessitaremos de um arquivo .xml que define o layout do nosso widget.