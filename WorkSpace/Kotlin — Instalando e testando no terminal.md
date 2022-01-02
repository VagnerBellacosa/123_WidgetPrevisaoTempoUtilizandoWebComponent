# Kotlin — Instalando e testando no terminal

[![Nando Kstro Net](https://miro.medium.com/fit/c/96/96/1*vyI_jdR0020qIqrb0BvmgQ.jpeg)](https://nandokstronet.medium.com/?source=post_page-----b1b34606c7b4-----------------------------------)

[Nando Kstro Net](https://nandokstronet.medium.com/?source=post_page-----b1b34606c7b4-----------------------------------) - [Jul 6, 2017](https://blog.codeexpertslearning.com.br/kotlin-instalando-e-testando-no-terminal-b1b34606c7b4?source=post_page-----b1b34606c7b4-----------------------------------) · 2 min read

Fala galera! Neste post vamos baixar e instalar o compiler do Kotlin em nosso terminal! Será um post bem rápido já introduzindo pra uma série de posts sobre a linguagem que virão a seguir!

Ao instalar o compiler em nosso terminal, teremos a mão o shell interativo do Kotlin, no qual poderemos realizar alguns testes e executar alguns scripts da linguagem!

# MAC

No OS X certifique-se de ter o [brew](https://brew.sh/index_pt-br.html) instalado em sua máquina! O brew é um gerenciador de pacotes para OS X. Uma vez estando com o brew em seu sistema, execute os comandos abaixo:

```
$ brew update
$ brew install kotlin
```

# Linux

No linux vamos utilizar o sdkman.io, recomendado pela própria documentação do Kotlin. É bem simples também, basta seguir os comandos abaixo:

```
$ curl -s https://get.sdkman.io | bash
$ sdk install kotlin
```

Certifique-se de reiniciar seu terminal para ter acesso aos command lines instalados!

# Windows

No Windows você pode baixar o zip com o compiler [aqui](https://github.com/JetBrains/kotlin/releases/tag/v1.1.3-2), descompacte em sua pasta de escolha e adicione a pasta `bin` no path do seu sistema. Uma vez feito isso, utilize o cmd do Windows para testar os comandos que mostrarei a seguir!

> Caso queira baixar o zip ele possui binarios para todos os sistemas!

# Hello World!

Vamos, rapidamente, executar nosso Hello World! O que vamos precisar nesse momento é do `kotlin-jvm` , então, em seu terminal digite `kotlin-jvm` , obtendo o resultado abaixo:

![img](https://miro.medium.com/max/60/1*hg4j0Fxx7hoI_riwWJIOJA.png?q=20)

![img](https://miro.medium.com/max/700/1*hg4j0Fxx7hoI_riwWJIOJA.png)

Kotlin em modo interativo

Execute o código abaixo em seu Kotlin Shell, aberto como resultado do comando executado anteriormente:

```
println("Hello, World!")
```

Chegando no resultado abaixo:

![img](https://miro.medium.com/max/60/1*P8C2gtvh4uhqveaDWdFuuA.png?q=20)

![img](https://miro.medium.com/max/700/1*P8C2gtvh4uhqveaDWdFuuA.png)

Hello World no Kotlin Shell

# Conclusões

Você pode executar diversos testes no Kotlin Shell, aproveite pra testar e brincar com a linguagem Kotlin! Em nossos próximos posts entraremos nos conceitos base da linguagem e o Kotlin Shell será nosso braço direito nesses primeiros passos!