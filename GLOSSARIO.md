## **Construtor**

*  Os construtores são os responsáveis por criar o objeto em memória, ou seja, instanciar a classe que foi definida.
``` Java

public class Exemplo{
    
    public Exemplo(){
        System.out.println("Construtor");
    }
}

```

## **Instanciação**

* É um processo por meio do qual se realiza a cópia de um objeto(classe) existente.
 ``` Java

 public class Pessoa{
    
     public string nome;
     public char sexo;
     public int idade;
 }
 ```

 ## **Palavra reservada new**

 * Operador utilizado para criar um objeto, instância de uma classe. Trata de reservar memória o suficiente para o objeto e criar automaticamente uma referência a ele.
 ``` Java
 public class Casa{
     int comprimento;
     int altura;

     Casa(){
         comprimento = 20;
         altura = 3;
     }

     public static void main(String[]args){
         Casa objeto1 = new Casa();
         Casa objeto2;
         objeto2 = new Casa();
     }
 }

 ```

 ## **Palavra reservada instanceof**

 * Determina se um objeto é uma instância de determinada classe, superclasse ou interface.

## **Encapsulamento**

* É a técnica utilizada para esconder uma ideia, ou seja, não expôr detalhes internos para o usuário, tornando partes do sistema mais independentes possível.

## **Palavra reservada this**

* Variável de referência que diz respeito a instancia atual de um objeto.

## **Getters/Setters**

* Estes métodos são modificadores e seletores dos atributos da sua classe. Consiste em os atributos de uma classe não conseguirem ser acessados diretamente.
``` Java
public class Teste {
    private double soma;
    
    public void setSoma(double soma) {
        this.soma = soma;
    }
    
    public double getSoma() {
        return soma;
    }
}
```

## **Palavra reservada public/private**

* O modificador **public** deixará visível a classe ou membro para todas as outras classes, subclasses e pacotes do projeto Java.

* O modificador **private** deixará visível o atributo apenas para a classe em que este atributo se encontra.
``` Java 
public class PubPriv {
    public int atributoPublico;
    private int atributoPrivado;
}
```

## **Assinatura de método**

* Dois métodos tem a mesma assinatura se eles tiverem o mesmo nome e tipos de parâmetro, ou a seha é a junção do nome do método e os seus parâmetros tipados.
``` Java
public class AssMetodo {
    public void metodo(String x) {
    }
    public int metodo(Int x) {
        return 0;
    }
}
```

## **Sobrecarga de método**

* É um conceito do polimorfismo que consiste basicamente na criação de dois ou mais métodos com nomes totalmente iguais em uma classe. Permite que utilizemos o mesmo nome em mais de um método contanto que suas listas de argumentos sejam diferentes para que seja feita a separação dos mesmos.
``` Java
public class Somatoria{
    public double soma( double a, double b){
        return a+b;
    }
    public int calcula( int a, int b){
        return a+b;
    
    }

    public String soma( String a, String b){
        return a+b;
    }
}
```

## **Escopo de classe**

* Se refere à acessibilidade e a vida de uma variável. Quanto maior é o alcance depende de onde uma variável é declarada. Por exemplo, se uma variável é declarada na parte superior de uma classe, ela será acessível a todos os métodos de classe. Se for declarada num método, em seguida, só pode ser utilizada em tal método.

## **Palavra reservada final**
* É um método que não pode ser sobrescrito nas subclasses. Usado para garantir que um determinado algoritmo não possa ser modificado pelas subclasses.
``` Java

class Final {
    private int man;
    public final int man() {
        return man;
    }
    
}
```

## **Associação Simples**

* É quando uma classe possui um atributo vindo de outra classe. Atributo da Classe. Símbolo UML "<-------->"

## **Relacionamento de dependência**
* Ocorre quando uma classe utiliza os serviços de outra classe. Ocorre no método da classe. Símbolo UML "- - - - - >".

## **Relacinamento de Agregação**
* É quando duas classes têm uma relação todo-parte, a parte consegue existir sem o todo. Atributo da Classe. Símbolo UML "-------<>"

## **Relacionamento de Composição**
* É quando duas classes têm uma todo-parte, a parte não consegue existir sem o todo. Atributo da Classe. Símbolo UML "-------<//>"