# Introdução à Manipulação de Objetos em Java

Este exemplo simples demonstra como trabalhar com objetos em Java, especificamente com a classe ArrayList para armazenar e manipular uma lista de números inteiros.

```
import java.util.ArrayList;
import java.util.Collections;

public class Main {
    public static void main(String[] args) {
        ArrayList<Integer> numeros = new ArrayList<>();
        numeros.add(5);
        numeros.add(1);
        numeros.add(9);
        numeros.add(4);
        numeros.add(3);
        numeros.add(2);

        Collections.sort(numeros);
        System.out.println(numeros);
    }
}
```

# Explicação do Código

### Criando um Objeto ArrayList

```
ArrayList<Integer> numeros = new ArrayList<>();
```

- new ArrayList<>() cria um novo objeto do tipo ArrayList na memória.
- ArrayList<Integer> numeros declara uma variável chamada numeros que pode armazenar um ArrayList de inteiros.
- O ArrayList é um tipo de coleção que pode redimensionar automaticamente e permite operações dinâmicas de inserção e remoção de elementos.

### Adicionando Elementos ao ArrayList

```
numeros.add(5);
numeros.add(1);
numeros.add(9);
numeros.add(4);
numeros.add(3);
numeros.add(2);
```

- numeros.add(valor) adiciona o valor especificado ao final do ArrayList.
- Após essas operações, a lista numeros conterá [5, 1, 9, 4, 3, 2].

### Imprimindo o ArrayList sem Ordenação

```
System.out.println(numeros);
```

Isso imprimirá a lista na ordem em que os elementos foram adicionados: [5, 1, 9, 4, 3, 2].

### Ordenando o ArrayList

```
Collections.sort(numeros);
```

- Collections.sort(numeros) ordena a lista numeros em ordem crescente.
- A função sort modifica o próprio objeto numeros, portanto, não é necessário armazenar o resultado em uma nova variável.

### Imprimindo o ArrayList Ordenado

```
System.out.println(numeros);
```

Após a ordenação, isso imprimirá a lista em ordem crescente: [1, 2, 3, 4, 5, 9].

# Conclusão

Neste exemplo, vimos como criar e manipular um objeto ArrayList em Java. Criamos uma lista de números inteiros, adicionamos elementos a ela, imprimimos a lista, ordenamos os elementos e, finalmente, imprimimos a lista ordenada. O uso de Collections.sort para ordenar a lista demonstra como métodos podem operar diretamente sobre objetos, modificando-os sem a necessidade de criar novas instâncias.
