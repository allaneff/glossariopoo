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
 ``` Java
 /*Colocar exemplo*/
 ```

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

