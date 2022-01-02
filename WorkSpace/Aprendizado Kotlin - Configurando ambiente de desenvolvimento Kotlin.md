# Aprendizado Kotlin - Configurando ambiente de desenvolvimento Kotlin

21 Apr 2020 » [kotlin](https://antoniolazaro.dev/category/kotlin) (aproximadamente 3 minutos de leitura)

<iframe id="twitter-widget-0" scrolling="no" frameborder="0" allowtransparency="true" allowfullscreen="true" class="twitter-share-button twitter-share-button-rendered twitter-tweet-button" title="Twitter Tweet Button" src="https://platform.twitter.com/widgets/tweet_button.8f764d5bd2778f88121d31d7d8d8e1e3.en.html#dnt=false&amp;id=twitter-widget-0&amp;lang=en&amp;original_referer=https%3A%2F%2Fantoniolazaro.dev%2Fkotlin%2F2020%2F04%2F21%2Festudo-kotlin-parte2.html&amp;size=m&amp;text=Aprendizado%20Kotlin%20-%20Configurando%20ambiente%20de%20desenvolvimento%20Kotlin%20-%20Site%20pessoal%20de%20Antonio%20Lazaro%20(Popete)&amp;time=1643286019043&amp;type=share&amp;url=https%3A%2F%2Fantoniolazaro.dev%2Fkotlin%2F2020%2F04%2F21%2Festudo-kotlin-parte2.html&amp;via=antonio_lazaro" style="box-sizing: border-box; position: static; visibility: visible; width: 73px; height: 20px;"></iframe>

 




[Conheça a série sobre Kotlin](https://antoniolazaro.dev/kotlin/2020/04/20/estudo-kotlin-indice-serie.html)

## Introdução

A [Plural Sight](https://www.pluralsight.com/offer/2020/free-april-month) está com uma promoção para o mês de abril onde os cursos da plataforma estão todos abertos devido a situação da COVID-19. Diante disso, me cadastrei na plataforma e fiz o curso [“Getting Started With Kotlin”](https://app.pluralsight.com/library/courses/8251eea9-5847-4881-bc94-1c3e0dc8b42e/table-of-contents) by [Kevin Jones](https://app.pluralsight.com/profile/author/kevin-jones) (conta dele no [twitter:](https://twitter.com/kevinrjones?lang=en)).

Meu primeiro contato com Kotlin foi durante a seleção da Jaya onde fiz um projeto usando [Kotlin e Gradle com Javalin, Koin e Exposed](https://github.com/antoniolazaro/octo-events).

O curso ele tem duração de 2h, e cobre uma introdução, fala um pouco sobre programação orientada a objetos, funcional, interoperabilidade Java x Kotlin e vice-versa, e fala sobre a ferramenta de testes Spek.

## Configurando ambiente desenvolvimento Kotlin em ambientes Unix based

Para quem não tem a JVM instalada, particulamente, acho a o [SDKMan](https://sdkman.io/) a melhor forma de configurar itens do ambiente Java para ambientes Unix based. Usuários de Windows, não sei se tem uma forma de configurar o SDKMan no Windows.

Segue passo a passo de como testar e configurar ambiente Kotlin em ambiente Unix based:

1- [Instalar o SDK Man](https://sdkman.io/install)
2- Usando Sdk Man, [instalar o Kotlin](https://sdkman.io/sdks#kotlin)
3- Você pode ver que a variável de ambiente KOTLIN_HOME foi setada através do comando

```
echo \$KOTLIN_HOME
```

4- Testar a instalação do Kotlin através do comando kotlinc. Deve aparecer conforme abaixo. ![img](https://antoniolazaro.dev/static/img/kotlin/kotlin-demo.png)

## Hello World

A forma mais fácil de testar Kotlin sem necessidade de instalar nenhum software é através do site da própria linguagem [Try Kotlin](https://try.kotlinlang.org/#/Examples/Hello, world!/Simplest version/Simplest version.kt) que est[a sendo considerado obsoleto e eles recomendam agora o [Kotlin Playground](https://play.kotlinlang.org/).

Arquivos de código-fonte Kotlin eles tem a extensão .kt. O hello World Kotlin pode ser feito da seguinte forma (pode ser executado diretamente no terminal ou salvo como arquivo):

```
fun main(args: Array<String>){
println("Hello, World")
}
```

Assim como no Java existe a função public static void main, em Kotlin essa função é o main, descrito acima. É como a JVM interpreta que o Kotlin executará um programa.

Para compilar via linha de comando será necessário digitar o comando abaixo no diretório onde o arquivo foi salvo.

```
kotlinc nome-arquivo-fonte.kt
```

Para converter esse código Kotlin em um jar executável da JVM é necessário rodar o comando abaixo:

```
kotlinc nome-arquivo-fonte.kt -include-runtime -d nome-binario-executavel.jar
```

## IDEs

Dificilmente, alguém utilizará para projetos reais a estrutura acima, de executar manualmente, compilar, etc. Normalmente trabalhamos com IDEs em projetos reais. Não testei no Netbeans porque, particulamente não conheço e não uso, porém para as 3 IDEs que tenho na minha máquina (Eclipse,IntelliJ e VSCode) vi que o Kotlin tem plugin e suporte.

- IntelliJ: Instalar plugin Kotlin
- Eclipse: Instalar no Market Place o plugin para Kotlin
- VsCode: Instalar o plugin para Kotlin (baixei o que tinha mais download em minha busca, que foi do editor: mathiasfrohlich)

## Conclusão

Até o momento, estou utilizando IntelliJ como IDE para programar em Kotlin e tenho gostado do resultado. Achei conceitualmente muito parecido com Java, porém mais simples. A interoperabilidade com Java é muito bem feita para os testes incialmente feitos.


[Conheça a série sobre Kotlin](https://antoniolazaro.dev/kotlin/2020/04/20/estudo-kotlin-indice-serie.html)

## Outras Fontes:

Compartilhe esse post: → 

<iframe id="twitter-widget-1" scrolling="no" frameborder="0" allowtransparency="true" allowfullscreen="true" class="twitter-share-button twitter-share-button-rendered twitter-tweet-button" title="Twitter Tweet Button" src="https://platform.twitter.com/widgets/tweet_button.8f764d5bd2778f88121d31d7d8d8e1e3.en.html#dnt=false&amp;id=twitter-widget-1&amp;lang=en&amp;original_referer=https%3A%2F%2Fantoniolazaro.dev%2Fkotlin%2F2020%2F04%2F21%2Festudo-kotlin-parte2.html&amp;size=m&amp;text=Aprendizado%20Kotlin%20-%20Configurando%20ambiente%20de%20desenvolvimento%20Kotlin%20-%20Site%20pessoal%20de%20Antonio%20Lazaro%20(Popete)&amp;time=1643286019097&amp;type=share&amp;url=https%3A%2F%2Fantoniolazaro.dev%2Fkotlin%2F2020%2F04%2F21%2Festudo-kotlin-parte2.html&amp;via=antonio_lazaro" style="box-sizing: border-box; position: static; visibility: visible; width: 73px; height: 20px;"></iframe>

 



#### Related Posts

- [Aprendizado Kotlin - Scope Functions](https://antoniolazaro.dev/kotlin/2020/06/11/estudo-kotlin-parte14.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - When, uma versão melhorada do switch do Java](https://antoniolazaro.dev/kotlin/2020/05/05/estudo-kotlin-parte13.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Função repeat](https://antoniolazaro.dev/kotlin/2020/05/05/estudo-kotlin-parte12.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Palavras chaves, identificadores, gramática e código-fonte da linguagem](https://antoniolazaro.dev/kotlin/2020/05/01/estudo-kotlin-parte11.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Ranges](https://antoniolazaro.dev/kotlin/2020/05/01/estudo-kotlin-parte10.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Exception](https://antoniolazaro.dev/kotlin/2020/04/22/estudo-kotlin-parte9.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))

[« Aprendizado Kotlin - Um pouco sobre Kotlin, minhas percepções do primeiro contato](https://antoniolazaro.dev/kotlin/2020/04/21/estudo-kotlin-parte1.html)[Aprendizado Kotlin - Alguns recursos da linguagem »](https://antoniolazaro.dev/kotlin/2020/04/21/estudo-kotlin-parte3.html)

<iframe id="dsq-app5637" name="dsq-app5637" allowtransparency="true" frameborder="0" scrolling="no" tabindex="0" title="Disqus" width="100%" src="https://disqus.com/recommendations/?base=default&amp;f=antoniolazaro-github-io&amp;t_i=https%3A%2F%2Fantoniolazaro.dev_Aprendizado%20Kotlin%20-%20Configurando%20ambiente%20de%20desenvolvimento%20Kotlin&amp;t_u=https%3A%2F%2Fantoniolazaro.dev%2Fkotlin%2F2020%2F04%2F21%2Festudo-kotlin-parte2.html&amp;t_e=Aprendizado%20Kotlin%20-%20Configurando%20ambiente%20de%20desenvolvimento%20Kotlin&amp;t_d=Aprendizado%20Kotlin%20-%20Configurando%20ambiente%20de%20desenvolvimento%20Kotlin&amp;t_t=Aprendizado%20Kotlin%20-%20Configurando%20ambiente%20de%20desenvolvimento%20Kotlin#version=8b0221d1e6088a6359fd494f934e58e6" horizontalscrolling="no" verticalscrolling="no" style="box-sizing: border-box !important; width: 730px; border: none !important; overflow: hidden !important; height: 0px !important; display: inline !important;"></iframe>