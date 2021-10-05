# Desenvolvimento com Android Studio. Aula 02 Widgets, Manipulação de Dados e Programação de Eventos



|      |      |
| ---- | ---- |
|      |      |

- [ SHARE](https://docplayer.com.br/14273366-Desenvolvimento-com-android-studio-aula-02-widgets-manipulacao-de-dados-e-programacao-de-eventos.html#tab_1_1_1) - [ HTML](https://docplayer.com.br/14273366-Desenvolvimento-com-android-studio-aula-02-widgets-manipulacao-de-dados-e-programacao-de-eventos.html#tab_1_1_2) - [ DOWNLOAD](https://docplayer.com.br/14273366-Desenvolvimento-com-android-studio-aula-02-widgets-manipulacao-de-dados-e-programacao-de-eventos.html#download_tab_content)



1 Desenvolvimento com Android Studio Aula 02 Widgets, Manipulação de Dados e Programação de Eventos

2 Widgets

3 TextView O Widget TextView é utilizado para apresentar um texto não editável na tela. Qualquer componente gráfico pode ser adicionado arrastando da paleta até a tela gráfica ou criando o código XML deste elemento. O código XML que representa um TextView pode ser representado: <TextView /> android:layout_width="wrap_content" android:layout_height="wrap_content android:text="texto 1:

4 TextView Propriedades: android:text= Texto 1": Este parâmetro define o texto que é exibido na TextView : Este parâmetro define um identificado textview. Caso seja necessário manipular este elemento via código Java, usamos este identificador para acessá-lo OBS: De acordo com a documentação do android é considerado uma boa prática exteriorizar strings, arrays de string, imagens, cores, e outros recursos que você ou outra pessoa possa gerenciá-los separadamente do código de seu aplicativo. Para isto, adicione uma nova String: res -> values -> strings <string name="nome">nome</string> Em seguida configure o parâmentro android:text conforme abaixo:

5 TextView Propriedades adicionais: android:textcolor="#a5b6c7 : Este parâmetro define uma cor ao texto exibido. A cor definida deve está em formato hexadecimal. android:textsize="20dp : Este parâmetro define o tamanho do texto. android:textstyle="bold : Define o estilo do texto(negrito, itálico ou normal) android:textallcaps="true : Define se o texto exibido aparecerá em caixa alta (true) ou em caixa baixa(false) android:layout_gravity="center_horizontal : Define o alinhamento do texto android:typeface="serif : Define os padrões de fonte, ou famílias, que no caso do Android são 3 famílias: Droid Sans, Droid Sans Mono e Droid Serif

6 TextView Propriedades: android:shadowcolor: cor da sombra android:shadowradius: o raio da sombra android:shadowdx: o distanciamento horizontal da sombra em relação ao texto android:shadowdy: o distanciamento vertical da sombra em relação ao texto

7 ImageView O Widget ImageView é usado para adicionar uma imagem em uma activity(tela) Os parâmetros id, gravity, e outras propriedades comuns a todos os widgets são configurados da mesma forma aos já apresentados Definindo a imagem (propriedade src): OBS: Antes de utilizar uma imagem, é necessário coloca-la na pasta de Para isto copie e cole a imagem na pasta específica. <ImageView android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_centerhorizontal="true" />

8 ImageView

9 EditText Um EditText é um componente gráfico que permite ao usuário interagir com o aplicativo através da inserção de textos. Quando o usuário tocar em um EditText, automaticamente será exibido o teclado virtual para que uma informação seja passada. Na paleta de Widgets é possível incluir EditText com entradas préconfiguradas para permitir apenas números, campos no formato senha(password), etc. Uma EditText também poderá ser adicionada via código XML, conforme abaixo: <EditText android:layout_width="wrap_content" android:layout_height="wrap_content" android:layout_alignparenttop="true" />

10 EditText

11 EditText Exibindo ajuda: android:hint: este atributo exibe uma dica dentro de um componente EditText, a qual ajuda o usuário a entender o objetivo do componente. Quando o usuário iniciar a digitação neste componente, a dica de ajuda desaparece.

12 Button Um Button é um componente gráfico que permite ao usuário interagir com o aplicativo através de cliques(toques) no botão. Em geral os botões acompanham código JAVA que é acionado para realizar uma determinada função assim que o usuário do aplicativo toca-lo. Usamos para isto a propriedade onclick para chamar uma função no código JAVA a qual o formulário está relacionado. As propriedades id, text, background, margin e outras propriedades comuns a todos os widgets são configuradas da mesma forma que os controles apresentados <Button android:layout_width="wrap_content" android:layout_height="wrap_content" android:text="new Button" android:layout_centerhorizontal="true" />

13 Button

14 Relacionando Widgets no código Java

15 Manipulando Widgets através de código JAVA Para manipular os componentes que adicionamos via XML é necessário um código JAVA que esteja relacionado com a interface gráfica do aplicativo. Na programação em Android, temos em geral um arquivo.xml que contém o layout e interface gráfica do aplicativo e uma classe JAVA associada a uma Activity. Ao criar um novo projeto para Android, foi criado automaticamente pela ferramenta um Layout.XML ( res -> layout -> nome do layout.xml) e uma classe Java ( src > nome do pacote -> nome da classe.java Observe que na classe JAVA, existe um método OnCreate: public class Aula02Activity extends Activity protected void oncreate(bundle savedinstancestate) { super.oncreate(savedinstancestate); setcontentview(r.layout.activity_aula02); }

16 Manipulando Widgets através de código JAVA O método oncreate(bundle) é onde você inicia sua atividade e define a interface gráfica a qual está relacionada através do método setcontentview. Assim podemos obter os widgets (elementos de tela) através de um método chamado findviewbyid(). Para que um arquivo.java consiga se comunicar com o layout XML e outros recursos, existe uma classe intermediária, criada e atualizada automaticamente pela ferramenta, responsável por realizar esta ligação. Esta classe é chamada de R.Java. Observe que o método setcontentview relaciona a interface gráfica usando a classe R: (setcontentview(r.layout.activity_main);

17 Manipulando Widgets através de código JAVA O método oncreate() - É a primeira função a ser executada em uma Activity (Tela). Geralmente é a responsável por carregar os layouts XML e outras operações de inicialização. É executada apenas uma vez. O método oncreate() é importante pois é nele que iniciaremos nossos objetivos visuais e relacionamos os eventos(onclick,ontouch, etc) Neste método, programamos todas as funções que gostaríamos que fossem inicializadas quando o aplicativo for executado. OBS: Este método só é executado uma única vez, no início da aplicação.

18 A classe R.Java Esta classe é o coração do sistema Android. Ela representa, em forma de atributos Java, todos os recursos da sua aplicação que estão dentro dos diretórios já explicados de um aplicativo Android. Ela é gerada e atualizada automaticamente e não deve ser editada manualmente; o Eclipse fará isto automaticamente. Por exemplo, temos dentro do diretório res/drawable a imagem icon.png ; podemos acessá-la de dentro da nossa aplicação Android com a seguinte expressão: R.drawable.icon, onde R é a classe, drawable é o diretório e icon é o nome do recurso. Isto serve para quaisquer recursos presentes dentro dos diretórios de recursos.

19 Manipulando Widgets através de código JAVA Os widgets podem ser usados no nosso código Java. Se no código XML tivermos um widget do tipo EditText, para acessar esse componente pelo Java, é preciso fazer uso da classe EditText. Cada widget no XML possui o seu respectivo em classe Java, logo, se possui um widget TextView, para acessa-lo devemos fazer uso da classe TextView e assim vai. Podemos relacionar um widget a qualquer momento(oncreate, no clique de um botão, etc.) No exemplo abaixo, associamos os widget no método oncreate da activity: TextView tvboasvindas; tvboasvindas = (TextView)findViewById(R.id.tvBoasVindas); EditText txtnome; txtnome = (EditText)findViewById(R.id.txtNome);

20 Manipulando Widgets através de código JAVA O código abaixo cria um objeto do tipo EditText no código Java EditText txtnome; Para relacionar o objeto criado com o seu respectivo correspondente na interface gráfica usamos o método findviewbyid e especificamos qual elemento está relacionado através da classe R.id. Como JAVA é uma linguagem fortemente tipada, faz-se obrigatório converter o elemento para o tipo correto de dado, e isto é feito fazendo o casting (EditText), (TextView), etc. txtnome = (EditText) findviewbyid(r.id.txtnome); Este processo é feito semelhantemente para quaisquer recursos presentes dentro da interface gráfica XML.

21 Programando Eventos Botões e Ações

22 Programando eventos A programação para Android, semelhantemente a outros ambientes, linguagens e ferramentas gráficas, é orientada a eventos, neste caso, aos cliques e toques na tela. Cada vez que um usuário clica em um botão, seleciona um item em uma lista, ou pressiona uma tecla, o sistema operacional gera um evento Se uma aplicação está interessada em um evento específico (por exemplo, clique em um botão), deve solicitar ao sistema para escutar o evento. Se a aplicação não está interessada, seu processamento continua de forma normal. É importante observar que a aplicação não espera pela ocorrência de eventos isso é controlado pelo sistema.

23 Programando eventos Para que um componente ou container possa escutar eventos, é preciso instalar um listener. Listeners são classes criadas especificamente para o tratamento de eventos. Um event listener é uma interface da classe View que contém um método simples de chamada. Esse método pode ser chamado pela framework Android quando a View a qual o listener está registrado é chamado por uma interação de usuário com um item da interface, ou seja, quando a ação correspondente ocorre no objeto. Por exemplo, quando um botão é clicado, o método onclick() é chamado no objeto.



24 Programando eventos Os principais eventos presentes na programação para Android são: onclick() Vem de View.OnClickListener. É chamado quando o usuário toca o item (quando estiver em modo de toque) ou foca o item através de teclas de navegação ou trackball e pressiona o botão de enter correspondente ou pressiona o trackbak (que também serve como enter). onlongclick() Vem de View.OnLongClickListener. É chamado quando o usuário toca um item e o segura (quando estiver em modo de toque) ou foca o item através de teclas de navegação ou trackball e pressiona o botão de enter correspondente e o segura ou pressiona o trackbak por pelo menos um segundo.

25 Programando eventos Os principais eventos presentes na programação para Android são: onfocuschange() Vem de View.OnFocusChangeListener. É chamado quando o usuário navega para dentro ou para fora de um item, usando as teclas de navegação ou trackball. onkey() Vem de View.OnKeyListener. É chamado quando o usuário foca em um item e pressiona ou solta uma tecla no dispositivo. Exemplo: quando se está escrevendo uma mensagem, você pode tocar no botão virtual (ou físico) da letra A e, ao soltá-lo, a letra A é mostrada na tela.

26 Programando eventos Os principais eventos presentes na programação para Android são: ontouch() Vem de View.OnTouchListener. É chamado quando o usuário performa uma ação qualificada como um evento de toque, incluindo pressionar, soltar ou qualquer movimento de gesto na tela (dentro dos limites do item). oncreatecontextmenu() Vem de View.OnCreateContextMenuListener. É chamado quando um menu de contexto está sendo criado (como resultado de um long click).

27 Atividade Verificar Idade Para exemplificar os listeners relacionados aos eventos, construa um layout semelhante ao apresentado ao lado. Este layout contém um TextView, um EditText e um Button Neste aplicativo chamaremos dois listener: onclick para o botão verificar idade

28 Atividade Verificar Idade Para referenciar os objetos: configure o nome das variáveis para : txtidade -> EditText btverificaridade -> Button Assim, nosso código para acessar os componentes fica: EditText txtidade = (EditText) findviewbyid(r.id.txtidade); Button bt = (Button) findviewbyid(r.id.btverificaridade);

29 Atividade Verificar Idade Após a criação do layout mostrado no exemplo anterior será programado um listener referente ao botão VERIFICAR IDADE. O listener com o evento deverá ser programado fora do método oncreate. Para tanto usaremos classe Anônima e o método setonclicklistener: bt.setonclicklistener( new View.OnClickListener() public void onclick(view v) { //Codigo } });

30 Atividade Verificar Idade Dentro do método public void onclick(view v) escreveremos o código associado ao clique. Neste caso, faremos um código para verificar a idade e classificar o valor informado e faixa etária(criança, adolescente, adulto) Usaremos a estrutura if...else para verificar uma faixa de idade(criança, adolescente e adulto) Ao final, exibiremos a faixa etária utilizando a classe Toast.

31 Atividade Verificar Idade Para exemplificar os listeners relacionados aos eventos, construa um layout semelhante ao apresentado ao lado. Este layout contém um TextView, um EditText e um Button Neste aplicativo chamaremos dois listener: onclick para o botão verificar idade



32 Atividade Verificar Idade bt.setonclicklistener( new View.OnClickListener() public void onclick(view v) { EditText txtidade = (EditText) findviewbyid(r.id.txtidade); int idade = Integer.parseInt(txtIdade.getText().toString()); String faixaetaria; if ((idade > 0) && (idade <= 12)) faixaetaria = "Criança"; else if ((idade > 12) && (idade <= 18)) faixaetaria = "Adolescente"; else faixaetaria = "Adulto"; }); } //A classe Toast é usada para mostrar uma mensagem na tela Toast.makeText(getBaseContext(), "Você é um(a) " + faixaetaria, Toast.LENGTH_SHORT).show();

33 Atividade Verificar Idade

34 Exercício - IMC Desenvolver um programa em Android para calcular o IMC. Os dados de entrada serão o peso e a altura. Um botão mostrará o resultado do cálculo da seguinte fórmula: IMC = PESO/ALTURA²