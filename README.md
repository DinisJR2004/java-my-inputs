# Ler - Biblioteca de Entrada de Dados em Java

## Descrição

O **Ler** é uma classe Java utilitária que fornece métodos para facilitar a leitura de diferentes tipos de dados a partir da entrada padrão (teclado). Essa classe evita a necessidade de tratar exceções repetitivamente ao ler entradas do usuário.

## Funcionalidades

- Leitura de **String**
- Leitura de **int**
- Leitura de **byte**
- Leitura de **short**
- Leitura de **long**
- Leitura de **float**
- Leitura de **double**
- Leitura de **char**
- Leitura de **boolean**

Todos os métodos lidam com exceções e garantem que o usuário insira um valor válido.

## Como Usar

1. **Baixe ou copie a classe **``** para seu projeto.**
2. **Importe a classe **``** no seu código:**
   ```java
   import myinputs.Ler;
   ```
3. **Use os métodos para capturar entrada do usuário:**
   ```java
   public class Main {
       public static void main(String[] args) {
           System.out.print("Digite um inteiro: ");
           int numero = Ler.umInt();
           System.out.println("Você digitou: " + numero);
       }
   }
   ```

## Exemplo Completo

```java
import myinputs.Ler;

public class ExemploUso {
    public static void main(String[] args) {
        System.out.print("Digite uma string: ");
        String texto = Ler.umaString();
        
        System.out.print("Digite um inteiro: ");
        int numero = Ler.umInt();
        
        System.out.print("Digite um float: ");
        float valor = Ler.umFloat();
        
        System.out.println("String digitada: " + texto);
        System.out.println("Inteiro digitado: " + numero);
        System.out.println("Float digitado: " + valor);
    }
}
```

## Observações

- Os métodos utilizam `BufferedReader` para capturar a entrada do usuário.
- Cada método repete a solicitação até que o usuário forneça um valor válido.
- O método `umChar()` retorna apenas o primeiro caractere da entrada.

## Licença

Este projeto está disponível sob a licença MIT. Sinta-se à vontade para usar, modificar e distribuir.

## Autor

Desenvolvido por DinisJR2004

