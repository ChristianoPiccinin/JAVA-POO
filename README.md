# Glossário

* Construtor
* Instanciação
* Palavra reservada new
* Palavra reservada instanciof
* Encapsulamento
* Palavra reservada this
* Getters/Setters
* Palavra reservada public/private
* Assinatura de método
* Sobrecarga de método
* Escopo de classe
* Escopo de objeto
* Palavra reservada final
* Relacionamento de dependência
* Relacionamento de Agregação
* Relacionamento de Composição


# Construtor

R: Os construtores são os responsáveis por criar o objeto em memória, ou seja, instanciar a classe que foi definida.
```java
public class Pessoa{
	/* construtor da classe Pessoa  */
	public Pessoa(){

	}
}
```

# Instanciação

R: A instanciação realiza uma cópia de um objeto existente. Dessa forma podemos utilizar a função de uma outra classe em nosso código.


```java
/*classe que será instanciada*/
public class Pessoa{
            public char   sexo;
            public string nome;
            public int    idade;
}


public class Aluno{
  static void Main() {
  	 /*instanciação da classe Pessoa*/
  	 Pessoa objAluno = new Pessoa();  
	 objAluno.sexo  = 'm';
	 objAluno.nome  = "Robert Baixo Serney";
	 objAluno.idade = 96;
  }
}

```

# Palavra reservada new

R: Usada para instanciar um objeto.
 
```java
public class Aluno{
  static void Main() {
  	 /*instanciação da classe Pessoa*/
  	 Pessoa objAluno = new Pessoa();  
  }
}
```

# Palavra reservada instanciof

R: Determina se um objeto é a instancia de uma classe, superclasse ou interface, desta forma é possivel comparar se o tipo da variavel é de uma determinada classe. 

```java
class Point   { int x, y; }
class Element { int atomicNumber; }
class Test {
    public static void main(String[] args) {
        Point   p = new Point();
        Element e = new Element();
        if (e instanceof Point) {  // compile-time error
            System.out.println("I get your point!");
            p = (Point)e;  // compile-time error
        }
    }
}
```

# Encapsulamento

R:  Encapsulamento é basicamente separar o programa em pequenas partes, o mais isolado possivel. 
# Palavra reservada this

R: Variável de referência que diz respeito a instancia atual de um objeto.

```java
public class Conta {
	int saldo = 0 ;
	public void setSaldo(int saldo) {
		this.saldo = saldo; 
    	}
}
```

# Getters/Setters

R: Os metodos **Getters** e **Setters** são usados para pegar as informações de variaveis que estão declaradas como **private**, dessa forma, gera mais segurança no código. 
```java
package greetings;

import javax.inject.Inject;
import javax.enterprise.context.RequestScoped;
import javax.inject.Named;

@Named
@RequestScoped
public class Printer {

    @Inject @Informal Greeting greeting;
    
    private String name;
    private String salutation;
		
    /*metodod de setter*/
    public void setName(String name) {
       this.name = name;
    }
    /*metodod de getter*/
    public String getName() {
       return name;
    }
}

```

# Palavra reservada public/private

R: A palavra reservada **public** faz com que uma classe, método ou variável possa ser acessado a partir de qualquer outra classe.

Já a palavra reservada **private** restringe a classe, método ou variavel somente de dentro da própria classe, desta forma não pode ser acessada atravez de outras classes.

```java
public class Pessoa{
	private int cpf;
	public String nome;
}
```

# Assinatura de método

R: Combinação do nome do método, tipos e ordem dos parâmetros.
```java
public void setIdade(int newIdade){
	idade = newIdade;
}
```

# Sobrecarga de método

R: A sobrecarga de métodos consiste basicamente em criar variações de um mesmo método, ou seja, a criação de dois ou mais métodos com nomes totalmente iguais em uma classe.

```java
public class calculadora{
 public int calcula( int a, int b){
    return a+b;
  }
  public double calcula( double a, double b){
     return a+b;
  }
   public String calcula( String a, String b){
     return a+b;
}
```
# Escopo de classe

R: O escopo é a visibilade de como a classe é vista pelos demais programas. 

# Escopo de objeto

R: O escope de objeto é a parte do programa onde as variaveis são acessiveis. Na tabela abaixo é possivel ver os tipos de classificação.

|Modifier  |Package | Subclass | World | 
|----------|--------|----------|-------|
|public    |  Yes   |   Yes    |   Yes |
|protected |  Yes   |   Yes    |   No  |
|Default   |  Yes   |   No     |   No  |
|private   |  No    |   No     |   No  |


# Palavra reservada final

R: Quando usada na definição de uma variável, significa que a variável não pode assumir outro valor, tornando-se uma constante. 

```java
public class PI {
    public static final double PI = 3.141592653589793;
}
```

# Relacionamento de dependência

R: Na classe de dependencia, uma classe necessita de uma outra classe. Por exemplo, Classe B depende de Classe A.

![Relacionamento de Dependecia](https://uploaddeimagens.com.br/images/001/473/658/original/dependencia.PNG)

# Relacinamento de Agregação

R: Nesse tipo de relacionamento, a principal função é  identificar a obrigatóriedade de uma complementação entre elas. 

![Relacionamento de Agregação](https://uploaddeimagens.com.br/images/001/473/661/original/agregacao.PNG)

# Relacionamento de Composição

R: Indica a representação entre a "Parte" e o "Todo", a parte só pode exister se compor o todo.

![Relacionamento de Composição](https://uploaddeimagens.com.br/images/001/473/657/original/composicao.PNG)

# Links:

(https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

(https://www.devmedia.com.br/o-que-significa-cada-palavra-reservada/8320)

(https://www.devmedia.com.br/encapsulamento-polimorfismo-heranca-em-java/12991)

(https://www.devmedia.com.br/conceitos-e-exemplos-instanciacao-estrutura-da-linguagem/18817)

(http://www.guj.com.br/t/o-que-e-instanceof/31561)

(https://docs.oracle.com/javase/specs/jls/se10/html/jls-15.html#d5e29775)

(http://www.guj.com.br/t/declaracao-da-variavel-de-objeto-e-comando-this/48874)
