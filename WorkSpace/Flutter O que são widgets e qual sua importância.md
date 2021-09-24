**[Flutter](https://www.treinaweb.com.br/blog/categoria/flutter)**

# Flutter: O que são widgets e qual sua importância

Veja neste artigo o que são e qual a importância dos widgets para a criação de interfaces no Flutter.

 cerca de 1 ano atrás

[Artigos](https://www.treinaweb.com.br/blog)Flutter: O que são widgets e qual sua importância

[O Flutter](https://www.treinaweb.com.br/blog/o-que-e-flutter/) é um framework desenvolvido pela Google para criação de aplicações móveis multiplataforma (Android e iOS) utilizando uma única base de código e muito clamado por sua facilidade em desenvolver aplicações com uma interface intuitiva e agradável. Para a criação destas interfaces, o Flutter utiliza um conceito de Widgets, como veremos neste artigo.

## O que são widgets?

Como dito anteriormente, toda interface de um aplicativo desenvolvido com o Flutter é criada com base em um conjunto de Widgets. Basicamente, um widget é um componente visual para definir a interface de um aplicativo.

Pense em uma tela do aplicativo como um LEGO, onde cada widget é uma pequena peça e, ao final, este conjunto de peças representará uma interface completa:

![img](https://dkrn4sk0rn31v.cloudfront.net/2020/05/15090303/lego-interfaces-flutter.png)

Para esse comportamento, o Flutter divide seus widgets em duas categorias:

- Layout: Widgets responsáveis por determinar a organização e posicionamentos de outros widgets. Estes widgets servem para delimitar áreas em nossas telas que serão preenchidos por outros widgets;
- Interface: Widgets responsáveis por criar componentes visuais que serão exibidos para os usuários. Estes widgets servem para determinar os componentes que comporão a interface do aplicativo.



![Flutter - Fundamentos](https://d2knvm16wkt3ia.cloudfront.net/assets/svg-icon/flutter.svg)

##### CursoFlutter - Fundamentos

[Conhecer o curso](https://www.treinaweb.com.br/curso/flutter-fundamentos)

### Widgets de Layout

Como dito anteriormente, os widgets de layout servem para determinar a estrutura da interface dos aplicativos e a organização de outros widgets que comporão a tela do app. Estes widgets são de grande importância no Flutter, já que uma estrutura bem definida de uma página é fundamental para a construção de sua interface.

O Flutter possui diversos widgets de layout, alguns dos principais são:

- [Scaffold](https://api.flutter.dev/flutter/material/Scaffold-class.html): Um widget responsável por criar um layout “padrão” para o app, contendo uma `appBar` e o conteúdo da tela.
- [Stack](https://flutter.dev/docs/development/ui/layout#stack): Widget responsável por “empilhar” widgets na tela do topo ao final da interface.
- [Container](https://flutter.dev/docs/development/ui/layout#container): Widget responsável por comportar novos widgets de layout. O Container é muito utilizado para comportar widgets em sua estrutura separando-os com bordas.

### Widgets de Interface

Diferente dos widgets de layout, os widgets de interface servem para criar componentes visuais que serão incorporados ao widgets de layout e, assim, organizados na tela. São componentes visuais, como botões, labels, icones, textos e qualquer outro componente que compõe a interface de um aplicativo.

O Flutter [possui centenas de widgets de interfaces](https://flutter.dev/docs/development/ui/widgets) documentados e prontos para serem utilizados em nossos aplicativos. Destes, podemos dar destaque para 2 conjuntos de widgets amplamente utilizados, o [Material](https://flutter.dev/docs/development/ui/widgets/material) e o [Cupertino](https://flutter.dev/docs/development/ui/widgets/cupertino). Basicamente, o Material é responsável por estilizar os widgets de interface com base nos padrões do [Material Design](https://www.treinaweb.com.br/blog/o-que-e-material-design/) da Google. Já o Cupertino é responsável por estilizar os widgets de interface com base nos padrões de design do iOS.

Vale lembrar que o time do Flutter é responsável pela construção e manutenção desses estilos, sendo assim, caso haja alguma mudança nos componentes destas plataformas, é questão de tempo até serem implementados no Flutter.

### Layout + Interface

Como vimos, os widgets de layout e interface são utilizados em conjunto. Basicamente, a construção de interfaces são compostos por widgets de interface inseridos em widgets de layout, como pode ser visto na imagem abaixo:

![img](https://dkrn4sk0rn31v.cloudfront.net/2020/05/14145719/construcao-widgets-interface-app.png)A imagem acima demonstra a combinação dos widgets de layout e interface para a construção de interfaces. É possível notar que os widgets de interface (botões, textos, icones) são “encaixados” nos widgets de layout (Column, Row).

- [#flutter](https://www.treinaweb.com.br/blog/tag/flutter)
- [#widgets](https://www.treinaweb.com.br/blog/tag/widgets)