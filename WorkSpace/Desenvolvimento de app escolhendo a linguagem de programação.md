# Desenvolvimento de app: escolhendo a linguagem de programação

**01/10/2020** às 16:00 - **14 min** de leitura

![Imagem de: Desenvolvimento de app: escolhendo a linguagem de programação](https://tm.ibxk.com.br/2020/10/01/01144131963267.jpg?ims=1120x420)

![Avatar do autor](https://www.tecmundo.com.br/desktop/assets/static/avatar-editor.svg)

Por: Ajay Chebbi.

Publicado em: 2 de julho de 2019.

Ao considerar as linguagens de programação, frameworks e SDKs para aplicativos móveis, você deve levar em conta o ambiente de desenvolvimento de front-end (UI), mas também estar atento ao ambiente de desenvolvimento de back-end (lado do servidor). Os desenvolvedores que estão codificando o front-end normalmente não são aqueles que estão codificando o back-end, mas em geral trabalham uns com os outros (atuam, afinal, em empresas). Nesse artigo, revisaremos as linguagens de programação e frameworks de desenvolvimento populares hoje em dia para o desenvolvimento de aplicativos e back-ends móveis.

### Tipos de aplicativos móveis

Considerando a perspectiva de codificação, desenvolvedores podem escolher criar um dentre três tipos de aplicativos móveis:

- Os aplicativos móveis nativos são aqueles escritos em uma linguagem que conta com suporte nativo do fornecedor do sistema operacional (OS) do dispositivo. As APIs fundamentais da plataforma estão 100% disponíveis para o código do aplicativo, e o sistema operacional fornece a biblioteca de componentes de UI. O processo de estruturação converte este código em um aplicativo executável com bytecode nativo do sistema operacional;
- Os aplicativos móveis multiplataforma são aqueles escritos em uma linguagem e que podem ser executados em todas as plataformas. Com aplicativos móveis multiplataforma, a linguagem usada para escrever seu aplicativo pode não ser a linguagem nativa do sistema operacional fundamental do dispositivo. Isso indica que o código pode estar em um padrão bridge, contido ou compilado ao bytecode, que pode ser executado diretamente no sistema operacional com a ajuda de algumas bibliotecas de suporte;
- Os web apps móveis são um paradigma leve em que uma URL é aberta no navegador do seu dispositivo, mas aparência e funcionamento se assemelham às de um aplicativo para celular padrão. Os sites móveis não são apresentados como um aplicativo instalado no dispositivo, mas são um paradigma importante a ser considerado durante o desenvolvimento para um dispositivo móvel. Os desenvolvedores podem usar dois paradigmas de programação de sites para criar web apps móveis:

- A programação responsiva é um estilo de programação de sites em que o layout do site se organiza para se adequar ao formato do dispositivo. Portanto, em vez de ter que navegar horizontalmente, o conteúdo “se encaixa” no lugar para se ajustar à amplitude do dispositivo. Esses sites também podem ser usados em um desktop. Aprenda sobre mais recentes [ideias de design responsivo](https://developer.ibm.com/articles/responsive-design-future/) no IBM Developer.
- A programação progressiva cria web apps progressivos que são sites normais; eles têm a aparência de um aplicativo móvel tradicional quando a navegação se dá a partir de um navegador em um dispositivo móvel, oferecendo uma experiência semelhante à de um aplicativo. Os web apps progressivos têm a capacidade de adicionar um link para a tela inicial (para que você obtenha um ícone do aplicativo) e também podem ser executados offline quando não se está conectado à internet, por meio do armazenamento local do conteúdo no dispositivo.

Você pode ler mais sobre os tipos de aplicativos no artigo “[Decidindo entre frameworks de programação de front-end móvel nativos e multiplataforma](https://developer.ibm.com/articles/deciding-between-native-and-cross-platform-mobile-frontend-programming-frameworks)”, do IBM Developer, 

### Desenvolvendo aplicativos móveis para a plataforma iOS

A plataforma iOS é uma plataforma proprietária feita pela Apple. A plataforma iOS está disponível para aparelhos celulares (iPhone) e tablets (iPad). Você pode desenvolver aplicativos para a plataforma iOS e direcionar o mesmo aplicativo tanto para um iPhone quanto para um iPad. Ao desenvolver o aplicativo, as limitações de espaço de cada um dos dispositivos devem ser levadas em conta. Os aplicativos para iOS podem ser instalados no seu iPhone ou iPad através da App Store da Apple.

Para desenvolver aplicativos para iOS, você precisa ter uma conta de desenvolvedor da Apple e o Xcode IDE em um computador Mac. Não há como desenvolver e realizar o processo de debugging (também chamado de depuração, em português) de maneira eficiente usando apenas uma máquina com sistema Windows. O Xcode inclui todo o kit de ferramentas de desenvolvimento da Apple necessárias: SDKs, um editor de código, ferramentas de compilação/construção, simuladores e um debugger (ferramenta também conhecida como depurador, em português). Você terá que usar CocoaPods ou Carthage como gerenciadores de pacotes para incorporar SDKs de terceiros ou enviar um SDK escrito por você.

Os aplicativos para dispositivos iOS podem ser desenvolvidos através do iOS SDK nativo com Objective-C e Swift ou com as várias tecnologias multiplataforma que são escritas no SDK desse framework, mas direcionadas para iOS.

### Objective-C

Objective-C foi a primeira linguagem suportada pela Apple para o desenvolvimento de aplicativos móveis do iOS. É uma linguagem orientada a objetos (OO) que deriva a sintaxe da linguagem de C e o aspecto OO de SmallTalk. Essa linguagem é comumente criticada por ter uma sintaxe aparentemente desajeitada, ser prolixa e apresentar colchetes que dificultam o processo de debugging. Todavia, é uma linguagem estável e madura, dado seu uso amplo ao longo de vários anos.

Desde que a Apple lançou o Swift, a popularidade do Objective-C diminuiu consideravelmente em novos desenvolvimentos móveis para iOS.

### Swift

A Apple lançou o Swift em 2014 como uma especificação de linguagem e o disponibilizou para o desenvolvimento de aplicativos móveis no Xcode em 2015. Após uma grande revisão da linguagem Swift em 2016 (v 3.0), o Swift superou o Objective-C como a linguagem para escrever aplicativos nativos do iOS. Embora Swift e Objective-C possam coexistir, isto é, bibliotecas escritas em Objective-C e utilitários em Objective-C podem ser usados em Swift, a Apple está deixando bem claro que o Swift é a nova escolha padrão para o desenvolvimento de aplicativos do iOS. O Swift é uma linguagem mais fácil, simples e compacta em comparação com Objective-C. Os desenvolvedores de Objective-C não devem ter problemas para migrar para o Swift.

- Explore o conteúdo do [hub de tecnologia Swift no IBM Developer](https://developer.ibm.com/technologies/swift/) e confira todas as diferentes maneiras de usar o Swift em seu desenvolvimento móvel.

### Desenvolvendo aplicativos móveis para a plataforma Android

O Android é uma plataforma de código aberto, desenvolvida e promovida principalmente pelo Google. O Google promove sua própria marca de dispositivo móvel, a Pixel (e a marca anterior, Nexus). No entanto, há um grande número de fabricantes, como Samsung, Huawei, Xiaomi e Oppo, que vendem suas próprias marcas de telefones e tablets com tecnologia Android e derivados do sistema operacional Android, como CyanogenMod e MIUI. Em se tratando de forma, os dispositivos Android estão disponíveis em uma multitude de dispositivos, desde telefones a tablets, pois há uma variedade de fabricantes com séries de modelos visando atender a diferentes preferências do usuário.

Para desenvolver aplicativos do Android, você precisa do kit de ferramentas de desenvolvimento do Android que contém o SDK, debuggers e emuladores necessários. Para um IDE, o [Android Studio](https://developer.android.com/studio/intro/) é de longe o mais popular, mas existem outros IDEs igualmente populares, como Netbeans e IntelliJ Idea. Você pode ter o ambiente de desenvolvimento em qualquer sistema operacional (Mac, Windows ou Linux). O Android usa o Gradle para o sistema de compilação, e o Android Studio disponibiliza modelos de código e outras ferramentas de avaliação e aprimoramento de desempenho.

Bibliotecas de terceiros são adicionadas ao aplicativo através de uma diretiva de pacote do Gradle. Um grande número de SDKs de terceiros no Android é distribuído com o uso de um gerenciador de pacotes chamado maven, popularmente conhecido como [mavencentral](https://mvnrepository.com/). Os aplicativos desenvolvidos para Android são distribuídos na loja padrão do Google Play, gerenciada pelo Google.

Os aplicativos podem ser desenvolvidos para dispositivos Android por meio do SDK nativo do Android com Java e Kotlin ou com as várias tecnologias multiplataforma que são escritas no SDK desse framework, mas direcionadas para iOS.

### Java

Java é a linguagem padrão para escrever aplicativos do Android desde que a plataforma Android foi introduzida, em 2008. É uma linguagem de programação orientada a objetos originalmente desenvolvida pela Sun Microsystems em 1995 (agora é propriedade da Oracle). Era uma linguagem muito popular como linguagem pura orientada a objetos (em comparação com C ++) e foi rapidamente adotada pela plataforma Android. A plataforma compila para "bytecode" interpretado de acordo com tempo de execução pela Java Virtual Machine (JVM) em execução no sistema operacional. Você escreve os aplicativos móveis em Java e programa no Android SDK. Os críticos da linguagem dizem que Java exige muito código “boilerplate” para executar uma tarefa simples, e conceitos como exceções são difíceis de entender. Até o momento, essa é a linguagem mais usada para o desenvolvimento de aplicativos do Android.

Apesar disso, a partir de 2019, Kotlin passou a ser a linguagem de preferência para desenvolvimento em Android, de acordo com o Google.

- Consulte a [introdução detalhada à programação Java](https://developer.ibm.com/series/intro-to-java-programming/) no IBM Developer para obter mais informações.

### Kotlin

Em 2017, o Google anunciou o suporte ao Kotlin como uma linguagem alternativa de alto desempenho para a programação em Android. Kotlin é interoperável com Java, e todas as bibliotecas Java podem ser acionadas por Kotlin. De maneira simplificada, pode-se dizer que Kotlin é uma forma mais organizada de Java. A curva de aprendizado de Java para Kotlin é suave. Quanto a nível de execução, o Kotlin compila para Bytecode Java.

- Saiba mais sobre Kotlin [na linha de aprendizagem em Kotlin](https://developer.ibm.com/series/learn-kotlin/) no IBM Developer.

### Desenvolvendo aplicativos móveis para ambas as plataformas iOS e Android

Em se tratando de abordagens de construção de aplicativos nativos, é necessário manter um código base por plataforma. O tamanho do repositório de código é proporcional às plataformas que precisam ser suportadas. Frequentemente, você precisa desenvolver para ambas as plataformas, mas não precisa dos recursos da linguagem nativa. Felizmente, existem tecnologias que permitem que você escreva em uma linguagem ou framework e direcione o aplicativo para ambas as plataformas, o que significa que aqueles desenvolvedores não familiarizados com Java e Swift mas especializados em outras tecnologias, como Web ou C#, podem usar suas habilidades para desenvolver aplicativos para Android e iOS.

Várias comunidades ou empresas de código aberto elaboraram frameworks que têm afinidade com suas bases de desenvolvedores para o desenvolvimento em Android e iOS. Esses frameworks são acompanhados de seus próprios ecossistemas de ferramentas e IDEs, oferecendo maior conveniência para os desenvolvedores familiarizados com eles. Por exemplo, o sistema de ferramentas em C# do Xamarin é voltado para o uso do Microsoft Visual Studio e o Apache Cordova é voltado para o uso de IDEs da web como o VSCode. Todavia, as ferramentas de ambiente de desenvolvimento para Android e iOS ainda devem estar instaladas (conforme explicado nas seções anteriores sobre Android e iOS) para que as ferramentas multiplataforma possam aproveitar os SDKs nativos e os pacotes. Às vezes, os frameworks incluem seus próprios simuladores, mas geralmente acabam por usar o simulador dos ambientes fundamentais de desenvolvimento nativo do Android ou iOS.

Os frameworks multiplataforma a seguir dependem de maven ou nuget para distribuir plug-ins e SDKs de terceiros. Alguns desenvolvedores também listam seus plug-ins para venda.

### HTML5 e Apache Cordova

O Apache Cordova teve início como um projeto da Adobe chamado PhoneGap. Com o Apache Cordova, você pode executar código HTML e JavaScript (JS) em uma instância segura do navegador (com uso de captive portal) chamada Webview. Usando um webview, você pode escrever código uma vez e, então, executá-lo em qualquer lugar. Uma das críticas à abordagem multiplataforma é que a resposta pode ser lenta devido à execução do código de JavaScript se dar no webview. Você pode ler mais sobre os pontos positivos e negativos dos frameworks de front-end móveis no artigo “[Decidindo entre frameworks de programação de front-end móvel nativas e multiplataforma](https://developer.ibm.com/articles/deciding-between-native-and-cross-platform-mobile-frontend-programming-frameworks)”, do IBM Developer.

O código HTML está incluído no próprio aplicativo e é instalado no dispositivo móvel. Isso possibilita o uso de uma ampla variedade de frameworks de UI da web como Jquery, React JS, Bootstrap, Angular JS ou Vue. Existem também outros frameworks em camadas adjacentes, como Ionic, que acabam por ser executados no Cordova. Além das bibliotecas de UI, há um conceito de plug-ins que permite que o código JS acesse recursos nativos do dispositivo, como câmera, lista de contatos ou localização. Um vasto ecossistema de plug-ins de terceiros está disponível.

O gerenciador de pacotes mais popular é o npm.

Os IDEs populares entre a comunidade de desenvolvedores são o Visual Studio Code e o Eclipse. O Ionic, que aparece como um wrapper no topo do Apache Cordova e atualmente usa Angular JS, também tem seu próprio IDE, disponível para compra, chamado Ionic Creator. No entanto, você ainda pode desenvolver um aplicativo com Ionic Angular JS usando qualquer outro IDE, conforme mencionado anteriormente.

- Conheça mais sobre o desenvolvimento de aplicativos móveis com o Apache Cordova no artigo “[O que é o Apache Cordova?](https://developer.ibm.com/articles/what-is-apache-cordova/)”, do IBM Developer.

### C# e Xamarin

C# é uma linguagem de programação orientada a objetos desenvolvida pela Microsoft. O framework do Xamarin (adquirido pela Microsoft) permite que você programe em C# no framework .NET, o qual é implementado na plataforma iOS por meio de uma implementação de código aberto chamada mono.

O IDE mais popular para escrever códigos em C# e no Xamarin é o Visual Studio Code da Microsoft. O código C# passa por compilação cruzada e é executado de forma nativa no dispositivo iOS ou Android. Isso permite uma execução sem atrasos muito próxima daquela do desenvolvimento nativo. Existem extensões especiais chamadas Xamarin.iOS e Xamarin.Android, as quais você pode usar para acessar recursos nativos do iOS e Android que podem ser chamadas a partir de C#. Para iOS, você precisa do XCode em um computador Mac para desenvolver o aplicativo iOS instalável.

### JavaScript e React Native

O React Native foi lançado em 2015 pelo Facebook, e utiliza JavaScript como linguagem de programação para escrever aplicativos móveis. Não se usa HTML para escrever aplicativos no React Native. Este código é então interpretado em tempo de execução e executado por meio de uma "ponte" para acessar os recursos nativos do SDK do dispositivo. Os aplicativos do React Native utilizam a biblioteca de UI nativa da plataforma para renderizar os componentes de UI, o que torna a UI verdadeiramente nativa. O React Native se tornou muito popular porque a curva de aprendizado para JavaScript é muito baixa.

- Comece a usar o React Native no artigo “[Dissecando o React Native](https://developer.ibm.com/articles/dissecting-react-native/)”, do IBM Developer.

### Dart and Flutter

Embora o Dart tenha sido divulgado pelo Google em 2011, o primeiro lançamento estável foi em 2017. Dart é uma linguagem de programação orientada a objetos. Você usa o framework do Flutter, do Google, para escrever aplicativos móveis para iOS.

Os IDEs mais populares são Android Studio, IntelliJ e Visual Studio Code (VSCode). Um dos recursos exclusivos do Flutter é que ele vem com sua própria biblioteca de frameworks de widgets de UI, que é baseada no Material Design, também do Google, bem como nos widgets de UI típicos do iOS.

### Desenvolvendo aplicativos móveis para a plataforma web

Embora não sejam um aplicativo instalado de fato, é importante considerar as UIs que são geradas ao navegar para um URL da web (ou seja, sites). Gerar sites tem algum valor para certos casos, como um aplicativo para eventos incidentais ou de curta duração, ou para capturar pequenas quantidades de informação como nome e endereço sem forçar um usuário a instalar um aplicativo. Com o advento dos progressive web apps (PWAs), a experiência do usuário em aplicativos e sites é indistinguível. Esses sites otimizados para celular são escritos utilizando tecnologias da web (HTML, JavaScript e CSS) e, normalmente, um framework de UI.

### Sites mobile otimizados

Usando qualquer um dos frameworks como Material, Bootstrap ou Foundation, você pode gerar um site responsivo. O web design responsivo conta com layouts que se adaptam ao espaço disponível através de uma experiência nativa. Por exemplo, um site pode ter um layout de 5 colunas quando acessado em um navegador de laptop, mas esse mesmo site será renderizado em um layout de 2 colunas quando visualizado em um navegador de um dispositivo móvel no modo retrato. As duas principais diferenças entre um site mobile otimizado e a visualização em um site normal em um telefone celular é que você não precisa aumentar o zoom para visualizar o conteúdo e não há rolagem horizontal.

### Progressive web apps (PWAs)

Os [progressive web apps](https://developer.ibm.com/clouddataservices/2016/11/08/building-offline-first-progressive-web-apps/) são, na verdade, sites renderizados como um aplicativo nativo. Os navegadores também evoluíram para detectar um PWA e remover o navegador adjacente para dar ao conteúdo da web o espaço total do dispositivo. Quando você adiciona um atalho para esse site, ele cria um ícone na tela inicial do celular, para que você possa iniciá-lo como um aplicativo normal. O navegador também armazena em cache localmente, no dispositivo, conteúdo especificado para que você tenha um tempo de carregamento rápido e confiável e também uma experiência offline progressiva. Isso é concretizado usando:

- Um service worker executado em segundo plano para pré-armazenar o conteúdo em cache;
- Design responsivo para otimização da renderização;
- Um manifesto do web app para notificar o navegador de que ele pode ser instalado.

### Conclusão

As plataformas móveis podem não passar por uma mudança drástica, com a exceção do aprimoramento de novos recursos por parte da Apple e do Google em suas respectivas plataformas, porém o cenário multiplataforma passou por muita turbulência. Você pode esperar que a cada ano haja um novo framework de preferência. É importante escolher a abordagem de desenvolvimento com base em habilidades coletivas e nos requisitos do aplicativo. Para ter sucesso no desenvolvimento móvel, os desenvolvedores precisam estar atentos às mudanças em ferramentas e plataformas, dado que o desenvolvimento móvel ainda é um espaço de tecnologia em evolução, com IA e machine learning chegando aos dispositivos móveis.

Bom desenvolvimento de aplicativos!

**...**

Quer ler mais conteúdo especializado de programação? Conheça o [IBM Blue Profile](https://www.tecmundo.com.br/desenvolvendo-com-ibm-cloud?utm_source=tecmundo&utm_medium=cta&utm_campaign=ibm-blue-profile) e tenha acesso a matérias exclusivas, novas jornadas de conhecimento e testes personalizados. Confira agora mesmo, consiga as badges e dê um upgrade na sua carreira!

**…..**

Quer dar o próximo grande passo na sua jornada profissional? Participe do [Cloud Training](https://www.ibm.com/br-pt/campaign/cloud-training), um curso online e gratuito que vai te preparar para o exame da certificação IBM Cloud Foundations. [Inscreva-se já](https://www.ibm.com/br-pt/campaign/cloud-training)!

## Categorias

[Software](https://www.tecmundo.com.br/software) [Programação](https://www.tecmundo.com.br/programacao) [IBMBlueProfile](https://www.tecmundo.com.br/ibmblueprofile) [IBMBackend](https://www.tecmundo.com.br/ibmbackend)