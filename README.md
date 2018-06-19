# Glossário

* Construtor

R: Os construtores são os responsáveis por criar o objeto em memória, ou seja, instanciar a classe que foi definida.
```java
public class Pessoa{
	/* construtor da classe Pessoa  */
	public Pessoa(){

	}
}
```

* Instanciação

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

* Palavra reservada new

R: Usada para instanciar um objeto.
 
```java
public class Aluno{
  static void Main() {
  	 /*instanciação da classe Pessoa*/
  	 Pessoa objAluno = new Pessoa();  
  }
}
```

* Palavra reservada instanciof

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

* Encapsulamento

* Palavra reservada this

R: Variável de referência que diz respeito a instancia atual de um objeto.

```java
public class Conta {
	int saldo = 0 ;
	public void setSaldo(int saldo) {
		this.saldo = saldo; 
    	}
}
```

* Getters/Setters

* Palavra reservada public/private

R: A palavra reservada **public** faz com que uma classe, método ou variável possa ser acessado a partir de qualquer outra classe.

Já a palavra reservada **private** restringe a classe, método ou variavel somente de dentro da própria classe, desta forma não pode ser acessada atravez de outras classes.


* Assinatura de método

* Sobrecarga de método

* Escopo de classe

* Escopo de objeto

* Palavra reservada final

R: Quando usada na definição de uma variável, significa que a variável não pode assumir outro valor, tornando-se uma constante. 

```java
public class PI {
    public static final double PI = 3.141592653589793;
}
```

* Relacionamento de dependência

* Relacinamento de Agregação

* Relacionamento de Composição



# Links:

(https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

(https://www.devmedia.com.br/o-que-significa-cada-palavra-reservada/8320)

(https://www.devmedia.com.br/encapsulamento-polimorfismo-heranca-em-java/12991)

(https://www.devmedia.com.br/conceitos-e-exemplos-instanciacao-estrutura-da-linguagem/18817)

(http://www.guj.com.br/t/o-que-e-instanceof/31561)

(https://docs.oracle.com/javase/specs/jls/se10/html/jls-15.html#d5e29775)

(http://www.guj.com.br/t/declaracao-da-variavel-de-objeto-e-comando-this/48874)
