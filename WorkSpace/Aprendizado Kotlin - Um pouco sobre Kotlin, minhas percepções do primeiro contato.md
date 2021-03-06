# Aprendizado Kotlin - Um pouco sobre Kotlin, minhas percepções do primeiro contato

21 Apr 2020 » [kotlin](https://antoniolazaro.dev/category/kotlin) (aproximadamente 5 minutos de leitura)

[Conheça a série sobre Kotlin](https://antoniolazaro.dev/kotlin/2020/04/20/estudo-kotlin-indice-serie.html)

## Introdução

Ontem iniciei um novo ciclo profissional e agora faço parte do time da [Jaya Tech](https://jaya.tech/) trabalhando para o [C6 Bank](https://www.c6bank.com.br/). Enquanto os acessos são criados/liberados, tive a oportunidade de ir me familiarizando mais com a linguagem utilizada no projeto que ficarei alocado. A principo a Stack trabalha com Kotlin e por esse motivo tenho que aprender a linguagem e conhecer suas características.

### Kotlin

Kotlin atualmente está na [versão 1.3.70](https://blog.jetbrains.com/kotlin/2020/03/kotlin-1-3-70-released/?_ga=2.196070380.1960498962.1587384907-1530203495.1584056577). A equipe trabalha na [release 1.4 que está em milestone 1](https://blog.jetbrains.com/kotlin/2020/03/kotlin-1-4-m1-released/?_ga=2.196070380.1960498962.1587384907-1530203495.1584056577).

Você pode testar recursos do Kotlin no [site da própria linguagem](https://kotlinlang.org/#try-kotlin) e ela tem uma [documentação rica e muito clara](https://kotlinlang.org/docs/tutorials/getting-started.html) com diversos tutoriais.

Uma boa fonte de informação sobre a linguagem, suas evoluções e usos é o [blog da linguagem](https://blog.jetbrains.com/kotlin/), bem como a [conta do Twitter](https://twitter.com/kotlin). Para conhecer os detalhes da linguagem, ela é open-source e pode ser conhecida internamente através da [conta do GitHub da JetBrains](https://github.com/JetBrains/kotlin), empresa responsável pela criação e manutenção do Kotlin. No github da [linguagem Kotlin](https://github.com/Kotlin), podem ser conhecidos diversos projetos complementares a linguagem com ferramentas e bibliotecas.

#### História Kotlin

Acredito eu, que a motivação da [JetBrains](https://www.jetbrains.com/) para criar uma nova linguagem de programação em relação ao Java devia ser uma inquietação em relação a lentidão da evolução da linguagem, bem como seu processo de release. Java nos últimos anos, ganhou status de “Old school” e isso obrigou o JCP a acelerar o processo de desenvolvimento do mesmo. Hoje temos releases semestrais do Java, seguindo a mesma cultura LTS (Long Term Support) que já existem em outros projetos Open Source. O ciclo de evolução ficou mais rápido com mudanças menores. Mas a JetBrains hoje tem um modelo de lançamento de release da linguagem mais livre do processo vinculado ao Java.

Em 2011, a JetBrains lançou a linguagem que recebeu o nome em homenagem a uma ilha russa de mesmo nome situada próxima a costa de São Pertesburgo onde a equipe do Kotlin reside. Essa ilha fica no lado ocidental da Russia, [próxima a Finlândia e a Estônia](https://goo.gl/maps/bhU78E8DyQGSLqh4A).

A linguagem teve fortes influências de [Scala](https://www.scala-lang.org/) e se pensou muito em interopibilidade com o Java, tanto que é possível misturar código Java com Kotlin e vice-versa.

Em 2017, no Google IO, a Google anunciou que essa se tornaria a linguagem oficial para o Android.

A partir de novembro de 2017, na versão 1.2, foi possível lançar uma release onde se programava código Kotlin para JVM e Javascript.

Na release 1.3, Kotlin trouxe o conceito de coroutines para programação assincrona.

Kotlin foi pensada para ser menos verbosa que o Java e mais produtiva. Fazendo o dev escrever menos código, consequentemente tendo mais tempo para pensar no negócio do que digitando.

## Ambiente de desenvolvimento

Por ser feito pela JetBrains, nos meus testes, minha perceção de melhor uso e produtividade no Kotlin é no InteliJ IDE. Porém Kotlin tem plugins para Eclipse e Visual Studio Code e funcionaram bem. Nesse primeiro contato o IntelliJ tem me agradado mais. Mesmo na versão Community Edition.

É possível também utilizar linha de comando para executar código Kotlin.

## Características

- Fortemente tipada: Como Java, porém de maneira mais simples devido a inferência de tipo.
- Inferência de tipo: Tipo não precisa ser declarado, ele é inferido na associação com o objeto.
- Concisa: Linguagem pensada para o dev escrever objetivamente seu código.
- Null Safe: Kotlin é pensada para evitar NullPointerException. Para declarar null a uma variável é necessário definir que a aquela variável suporta null explicitamente.
- Propósito geral: Mobile cross-platform, server side, native (windows/linux/mac), web development, - Android, data Science
- Interopelabilidade: Roda em qualquer ambiente JVM, no Browser e no Android. Suporta código Java, então bibliotecas e frameworks Java podem ser usado em ambiente/projetos Kotlin
- Tool-friendly: Suportada nas principais IDEs, inclusive na linha de comando.
- Funcional/Orientad a objetos: Suporta os dois paradigmas
- Extension functions: É possível se extender funcionalidades de uma classe sem usar herança
- Suporte a imutabilidade: Objetos podem ser considerados imutáveis (não podem sofrer nova atribuição) e esse recurso é muito importante quando falamos de programação funcional.
- Linguagem concisa para criação de DSLs (Domain Specification Language)
- Suporta funções como cidadãos de primeira classe e função de ordem superior [explicação melhor sobre os temas](https://leandromoh.gitbooks.io/tcc-paradigmas-de-programacao/5_paradigma_funcional/54_funcoes_de_primeira_classe_e_de_ordem_superior.html)

## Conclusão

Meu primeiro contato foi muito positivo com a linguagem e encontrei em Kotlin, recursos que sempre questionei porque o Java não tinha isso nativamente. Porém, entendo muito o dilema do Java de manter retrocompatibilidade, pensando no Enterprise que sempre foi o foco da linguagem. Construir uma linguagem sem essas amarras e dependências, permitiu a JetBrains a criar uma Java Clean e com práticas e decisões mais modernas. Eu não conheço C#, porém dizem que Kotlin tem muitas coisas boas que existem no C# nativamente. Acredito que toda ferramenta/linguagem que nasce depois, tem sempre a oportunidade de ser construída de maneira melhor e mais alinhada ao seu presente, que para linguagens mais antigas, teriam que tomar decisões de futuro para acertar o que temos hoje. Algumas coisas dão certo, outras não. Assim se caminha a humanidade, nada se cria, tudo se transforma, aprimora, evolui.

A ciência é algo muito bonito. Vamos valorizar.


[Conheça a série sobre Kotlin](https://antoniolazaro.dev/kotlin/2020/04/20/estudo-kotlin-indice-serie.html)

## Outras Fontes:

- https://www.treinaweb.com.br/blog/kotlin-a-nova-linguagem-oficial-para-desenvolvimento-android/
- https://www.androidpro.com.br/blog/kotlin/kotlin/
- https://blog.matheuscastiglioni.com.br/comecando-com-kotlin/
- https://cafeinacodificada.com.br/kotlin/
- https://en.wikipedia.org/wiki/Kotlin_(programming_language)


[Conheça a série sobre Kotlin](https://antoniolazaro.dev/kotlin/2020/04/20/estudo-kotlin-indice-serie.html)

Compartilhe esse post: → 

<iframe id="twitter-widget-1" scrolling="no" frameborder="0" allowtransparency="true" allowfullscreen="true" class="twitter-share-button twitter-share-button-rendered twitter-tweet-button" title="Twitter Tweet Button" src="https://platform.twitter.com/widgets/tweet_button.8f764d5bd2778f88121d31d7d8d8e1e3.en.html#dnt=false&amp;id=twitter-widget-1&amp;lang=en&amp;original_referer=https%3A%2F%2Fantoniolazaro.dev%2Fkotlin%2F2020%2F04%2F21%2Festudo-kotlin-parte1.html&amp;size=m&amp;text=Aprendizado%20Kotlin%20-%20Um%20pouco%20sobre%20Kotlin%2C%20minhas%20percep%C3%A7%C3%B5es%20do%20primeiro%20contato%20-%20Site%20pessoal%20de%20Antonio%20Lazaro%20(Popete)&amp;time=1643286566500&amp;type=share&amp;url=https%3A%2F%2Fantoniolazaro.dev%2Fkotlin%2F2020%2F04%2F21%2Festudo-kotlin-parte1.html&amp;via=antonio_lazaro" style="box-sizing: border-box; position: static; visibility: visible; width: 73px; height: 20px;"></iframe>

 



#### Related Posts

- [Aprendizado Kotlin - Scope Functions](https://antoniolazaro.dev/kotlin/2020/06/11/estudo-kotlin-parte14.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - When, uma versão melhorada do switch do Java](https://antoniolazaro.dev/kotlin/2020/05/05/estudo-kotlin-parte13.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Função repeat](https://antoniolazaro.dev/kotlin/2020/05/05/estudo-kotlin-parte12.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Palavras chaves, identificadores, gramática e código-fonte da linguagem](https://antoniolazaro.dev/kotlin/2020/05/01/estudo-kotlin-parte11.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Ranges](https://antoniolazaro.dev/kotlin/2020/05/01/estudo-kotlin-parte10.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))
- [Aprendizado Kotlin - Alguns recursos da linguagem - Exception](https://antoniolazaro.dev/kotlin/2020/04/22/estudo-kotlin-parte9.html) (Categories: [kotlin](https://antoniolazaro.dev/category/kotlin))

[« Aprendizado Kotlin - Índice da série - Organização dos posts](https://antoniolazaro.dev/kotlin/2020/04/20/estudo-kotlin-indice-serie.html)[Aprendizado Kotlin - Configurando ambiente de desenvolvimento Kotlin »](https://antoniolazaro.dev/kotlin/2020/04/21/estudo-kotlin-parte2.html)