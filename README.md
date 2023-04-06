# java ☕♨

## Estruturas e dados java.

### Tipos de dados java 🚩

---

Dados Primitivos 🎲 | Descrição 📋✏️
--------- | ------
BYTE | armazena 8 bits(1 byte) e recebe valores entre -128 á 127.É útil para armazenar valores que não exigem muita precisão, cálculos simples.
SHORT | armazena dados positivos e negativos e o dobro do BYTE(16 bits) e cobre 5 digitos. É útil para armazenar valores maiores do que os representáveis por um byte, mas também sem muita precisão.
INT | armazena dados positivos e negativos e o dobro do SHORT(32 bits) e cobre 10 digitos. É o tipo de dados mais comum para armazenar valores inteiros em Java, é o mais usado em operacõs matematicas.
LONG | armazena dados positivos e negativos e o dobro do INT(64 bits). É usado para armazenar valores maiores do que os representáveis por um int.
FLOAT | representa um número de ponto flutuante de precisão simples de (32 bits). É usado para representar números reais e útil para cálculos científicos.
DOUBLE | representa um número de ponto flutuante de precisão dupla de (64 bits). É usado para representar números reais com até 16 dígitos significativos e é mais preciso do que o float.
CHAR | representa um único caractere Unicode de (16 bits). É usado para armazenar letras, números, símbolos e outros caracteres de texto.
BOOLEAN | representa um valor que pode ser verdadeiro ou falso. É usado em operações de controle de fluxo para determinar quais caminhos de código seguir.

---

## Exemplos

---

## Int
1. Declare uma variável do tipo int:
```
int num;
```
2. Atribua um valor à variável:
````
num = 10;
```
3. ou combine a declaração e atribuição em:
```
int num = 10;
```
4. Utilize a variável em operações matemáticas:
````
int result = num + 5;

```
5. ou para exibir seu valor em um console:
```
System.out.println("Valor de num: " + num);

```
---
Dados de Referência 💡 |  Descrição 📋✏️
--------- | ------
STRING | representa uma sequência de caracteres. É usado para armazenar e manipular textos.
ARRAYS | representa uma coleção de elementos do mesmo tipo de dados. É usado para armazenar listas de valores, como uma lista de compras ou uma coleção de pontos em um gráfico.
CLASSES | representa um objeto de uma classe definida pelo usuário ou fornecida pelo próprio Java. É usado para criar instâncias de objetos e executar métodos nesses objetos.
 
---

### Estruturas condicionais em Java 🚩

---

Condicionais Java 📈 | Descrição 📋✏️
--------- | ------
IF | estrutura utilizada para testar condições, tem como objetivo executar uma ação apenas se a condição determinada for real.
ELSE | complemento do if, determina a ação que deve ser executada caso o condição seja falsa.
SWITCH/CASE | estrutura alternativa para códigos que necessitam de muitas condições e ficariam muito extensos ao usar if/else. Essa estrtura testa o valor da variavel com diversas opções e não apenas em 2 como no if/else, o "case" determina as diversas condições e quando uma corresponder ao valor da variavel, a condição será executada. A execução da condição é determinada pelo comando "break" e caso o valor da variavel não corresponda a nenhum case é executado o "default".

---

Loop Java 🔁 | Descrição 📋✏️
--------- | ------
FOR | estrutura de looping no qual o valor da variavel auxilia no controle da quantidade de vezes que a repetição será executada, o segundo determina até quando o comando será realizada e o terceiro indica até que ponto o valor da variavel será alterado antes que a repetição termine.
WHILE | estrutura de looping no qual não se sabe extamente quantas vezes a repetição será executada. Apens uma condição acompanha a sintaxe desse comando e enquanto ela não for verdadeira a repetição continuará acontecendo.
DO.. WHILE | estrutura de looping no qual um processo é repetido até que a condição determinada no final seja verdadeira, esse comando é usado no lugar do "while" pois a repetição é executada pelo menos 1 vez antes de checar se a condição é verdadeira ou falsa.
---
## Android Studio Google 🤖

---

### Elementos visuais do android 🚩

---

Elementos | Descrição 📋✏️
--------- | ------
BUTTON | Um elemento no qual o usuario pode clicar para executar uma ação.
TEXTVIEW | Um elemento que exibe um texto para o usuario.
EDITTEXT | Um elemento para inserir e editar texto. É necessario especificar um "inputType" para especificar o tipo de caracteres que devem ser recebidas.
LISTVIEW | Um elemento que realiza a exibição do conteudo em rolagem vertical de forma que a cada elemento adicionado é imediatamente colocado abaixo do anterior.
GRIDVIEW | Um elemento que realiza a exibição do conteudo em 2 dimensões sendoe elas, linhas e colunas. Os elementos são inseridos automaticamente usando o "ListAdapter" e definidos no layout bidimensional.
SCROOLVIEW | Elemento funciona como um scroll tanto vertical quanto horizontal para views. Além disso, também pode ser utilizado para ampliar ou diminuir conteudo adicionando outras propiedades. É recomendado utilizar esse elemento para poucos itens para que ele funcione em sua maior eficiência.
IMAGEVIEW | Elemento para exibição de imagens.
VIEWPAGER | Elemnto para gerenciar layout, ele permite que o usuario vire a tela para esquerda e direita. Além disso, também é possivel realizar o scroll horizontal.
DECORVIEW | Elemento permite marcar anotações e depois adicionar ao viewpager como recursos de layout.
ADAPTERVIEW | Elemento para exibir grandes conjuntos de dados.
RECYCLERVIEW | Elemento é uma melhoria dos elementos "listview" e "gridview" em questão de layout já que pode ser amplamente personalizado.
WEBVIEW | Elemento utilizado para exibir paginas web no aplicativo, geralmente usado para rodar o navegador ou conteudos do navegador no projeto.
VIDEOVIEW | Elemento utilizado para exibir arquivos de vídeo, ele permite que gerenciamento de layout e pode carregar de diversas fontes.
SEARCHVIEW | Elemnento fornece uma barra de pesquisa para o usuario que contém sugestões de pesquisa e resultados se estiverem previamente disponiveis.
VIEWANIMATOR | Elemento utilizado para alternar entre views, ele auxilia nas transições entre os "textviews","imageviews" ou qualquer outro view de layout. Ele alterna entre 2 ou mais views, o que fornece uma transição animada.
---

## Exemplos

---

### Button 🟢
1. Abra o arquivo e adicione o seguinte código para criar um botão:
```
<Button
    android:id="@+id/myButton"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Clique aqui"/>
```
2. Abra o arquivo MainActivity.java e adicione o seguinte código para lidar com o clique do botão:
```
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Button myButton = findViewById(R.id.myButton);
        myButton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Toast.makeText(MainActivity.this, "O botão foi clicado!", Toast.LENGTH_SHORT).show();
            }
        });
    }
}

``` 
### ImageView 🟡
1. Abra o arquivo e adicione o seguinte código para criar um ImageView:
 ```
 <ImageView
    android:id="@+id/myImage"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:src="@drawable/minha_imagem"/>
 ```
2. Abra o arquivo MainActivity.java e adicione o seguinte código para referenciar o ImageView:
```
public class MainActivity extends AppCompatActivity {

    private ImageView myImage;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        myImage = findViewById(R.id.myImage);
    }
}

```
### TextView 🔴
1. Abra o e adicione o seguinte código para criar um TextView:
```
<TextView
    android:id="@+id/myText"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Olá, mundo!"/>

```
2. Abra o arquivo MainActivity.java e adicione o seguinte código para referenciar o TextView
```
public class MainActivity extends AppCompatActivity {

    private TextView myText;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        myText = findViewById(R.id.myText);
    }
}

```











