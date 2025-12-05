

---

## **Masterclass Java: Dominando Testes Lógicos para Júnior**

**Duração:** 2 horas.

---

### **(15 min) | Módulo 1: Moldando a Mentalidade para o Sucesso**

**Instrutor:** "Olá, futuros(as) desenvolvedores(as)! Sejam muito bem-vindos. Antes de escrever uma única linha de código, vamos alinhar nossa mentalidade. Um teste de lógica não é um muro, é uma porta. Ele não quer te rejeitar, quer ver como você pensa, como você estrutura suas ideias e como você lida com um desafio sob pressão. Nosso objetivo nas próximas 2 horas não é decorar soluções, mas sim construir um **kit de ferramentas mental** para que vocês possam enfrentar *qualquer* problema com confiança e clareza."

**Tópicos a Abordar:**

*   **A Importância da Lógica sobre a Sintaxe:** O avaliador quer ver seu raciocínio. Um código com um pequeno erro de sintaxe, mas com uma lógica clara, vale mais do que um código perfeito que não resolve o problema.
*   **"Pense em Voz Alta":** A melhor forma de treinar é verbalizar seu processo. "Ok, eu preciso percorrer essa lista... para cada item, vou verificar se... se for verdadeiro, eu adiciono em outra lista...". Isso organiza o caos na sua mente.
*   **Erro é seu Amigo:** Num teste, você não tem um depurador (debugger). Seu erro é a sua única ferramenta de feedback. Não se desespere com um `NullPointerException` ou `ArrayIndexOutOfBoundsException`. Ele está te dizendo *exatamente* onde sua lógica quebrou. Aprenda a ler essas mensagens.

---

### **(60 min) | Módulo 2: O Arsenal do Desenvolvedor - Revisão de Conceitos-Chave**

**Instrutor:** "Agora, vamos revisar as ferramentas que estarão sempre à nossa disposição. Pensem nisso como um chef conhecendo seus facas. Cada uma tem um propósito específico e usar a certa no momento certo faz toda a diferença."

#### **1. Estruturas de Decisão e Repetição (10 min)**

*   **`if/else`:** O cérebro do seu programa. Domine as condições simples, compostas (`&&`, `||`) e aninhadas. **Dica de Ouro:** Para condições simples, conheça o operador ternário `(condicao ? valor_se_verdadeiro : valor_se_falso)`. Deixa o código mais limpo.
*   **`for`:** Seu carro de Fórmula 1. Perfeito para quando você sabe *exatamente* quantas vezes precisa repetir uma ação (ex: percorrer um array do início ao fim).
*   **`while`:** Sua caminhada na esteira. Você continua enquanto uma condição for verdadeira (ex: "enquanto o usuário não digitar 'sair'").

#### **2. Manipulação de Texto: `String` vs. `StringBuilder` (15 min)**

*   **`String`:** Imutável. Toda vez que você "modifica" uma String (`texto = texto + "a"`), o Java na verdade cria um NOVO objeto na memória. É ineficiente para muitas concatenações em um laço.
*   **`StringBuilder`:** Mutável. Ele modifica o objeto diretamente. É a ferramenta certa para construir strings dinamicamente dentro de laços.
    *   **Quando usar `StringBuilder`?** Sempre que você estiver concatenando strings em um loop.
    *   **Métodos Chave:** `append()` (adiciona no fim), `insert()` (adiciona em uma posição), `reverse()` (inverte), `toString()` (converte de volta para `String`).

#### **3. Arrays e a Classe `java.util.Arrays` (10 min)**

*   **Array:** Uma coleção de tamanho fixo. Seu tamanho não pode mudar depois de criado.
*   **Classe `Arrays`:** Seu canivete suíço para arrays. É uma classe de utilitários cheia de métodos estáticos.
    *   **Métodos Chave:** `Arrays.sort(meuArray)` (ordena), `Arrays.binarySearch(meuArray, valor)` (busca de forma eficiente, mas o array PRECISA estar ordenado antes), `Arrays.toString(meuArray)` (para imprimir o array de forma legível).

#### **4. A Joia da Coroa: Java Stream API (25 min)**

**Instrutor:** "Streams são a forma moderna e expressiva de lidar com coleções em Java. Em vez de dizer *como* fazer as coisas passo a passo (laço `for`), você diz *o que* quer fazer. É uma mudança de paradigma poderosa."

*   **O que é um Stream?** Uma sequência de dados que pode ser processada. Ele não armazena dados; ele os transporta.
*   **A Pipeline do Stream:** `Fonte -> Operações Intermediárias -> Operação Terminal`.
    *   **Fonte:** Onde vêm os dados? Um array, uma lista, etc. (`Arrays.stream(meauArray)`).
    *   **Operações Intermediárias:** Elas transformam o stream. São "preguiçosas" (lazy), só executam quando uma operação terminal é chamada.
        *   `filter(predicado)`: Filtra os elementos, mantendo apenas os que passam em um teste.
        *   `map(funcao)`: Transforma cada elemento em outra coisa (ex: de `String` para `Integer`).
        *   `sorted()`: Ordena os elementos.
    *   **Operação Terminal:** É o gatilho. Ela processa a pipeline e produz um resultado final.
        *   `forEach()`: Executa uma ação para cada elemento.
        *   `toArray()`: Coleta os resultados em um array.
        *   `sum()`, `count()`, `average()`: Fazem cálculos.
        *   `collect()`: Coleta os resultados em uma lista, set, etc.

---

### **(15 min) | Módulo 3: Estratégia de Batalha - Como se Preparar**

**Instrutor:** "Com as ferramentas em mãos, vamos à estratégia. Como vocês chegam no dia do teste prontos para vencer?"

1.  **Leia a Questão Duas Vezes:** A primeira vez para entender o objetivo geral. A segunda vez para pegar os detalhes: restrições, casos de exceção, formato de entrada e saída.
2.  **Desenhe o Problema:** Pegue um papel e caneta. Desenhe o array, a string, os passos. Visualizar ajuda a encontrar falhas na lógica antes mesmo de codificar.
3.  **Pense em Casos de Teste:** Antes de codificar, pense: "Se a entrada for vazia, o que acontece? Se for só um caractere? Se for um número negativo?". Isso te força a considerar os casos de exceção.
4.  **Comece Simples:** Escreva a versão mais simples e "burra" do código que funciona. Depois, se sobrar tempo, refine. Um código que funciona, mesmo que não seja o mais elegante, já te coloca no jogo.
5.  **Gerencie o Tempo:** Se ficar preso em um detalhe por mais de 10 minutos, avance. Volte para ele no final se sobrar tempo. É melhor entregar 4 questões 100% certas do que 1 questão perfeita e as outras incompletas.

---

### **(30 min) | Módulo 4: Desafio Final - 10 Testes Práticos**

**Instrutor:** "A teoria é fundamental, mas a prática faz o mestre. Aqui estão 10 desafios que simulam o que vocês encontrarão. Tentem resolver por conta própria. Depois, comparem com as soluções comentadas para entender diferentes abordagens."

---

### **Os 10 Testes Práticos**

**Teste 1: Cifra de César Simples**
Dada uma String e um número inteiro `n`, retorne uma nova String onde cada letra da original foi deslocada `n` posições para frente no alfabeto. (Ex: "abc", n=3 -> "def").

**Teste 2: Par com Menor Diferença**
Dado um array de inteiros e um número alvo `x`, encontre dois números no array cuja soma seja `x`. Se houver múltiplos pares, retorne aquele com a menor diferença absoluta entre eles.

**Teste 3: Palavra Mais Frequente**
Dada uma frase (String), retorne a palavra que mais aparece. Considere que as palavras são separadas por espaços e ignore maiúsculas/minúsculas ("a" e "A" contam como a mesma palavra).

**Teste 4: Número Palíndromo**
Dado um número inteiro, verifique se ele é um palíndromo. Um número é palíndromo se ele pode ser lido da mesma forma de trás para frente (ex: 121, 1331). Retorne `true` ou `false`.

**Teste 5: Inverter Palavras da Frase**
Dada uma frase, retorne uma nova frase com a ordem das palavras invertida, mas mantendo as palavras themselves intactas. (Ex: "Ola mundo" -> "mundo Ola").

**Teste 6: Soma de Preços com Stream**
Dada uma lista de produtos (classe `Produto` com `nome` e `preco`), use Java Streams para calcular a soma dos preços de todos os produtos cujo nome começa com a letra "A".

**Teste 7: Segundo Maior Número**
Dado um array de inteiros, encontre o segundo maior número. Não modifique o array original.

**Teste 8: Verificar Anagrama**
Dadas duas Strings, verifique se uma é um anagrama da outra. Um anagrama é uma reorganização das letras da outra palavra (ex: "listen" e "silent").

**Teste 9: Imprimir Padrão de Pirâmide**
Dado um número inteiro `n`, imprima uma pirâmide de `n` andares usando o caractere `*`.
Ex: n=3
  *
 ***
*****

**Teste 10: Soma dos Dígitos em uma String**
Dada uma String que pode conter letras e números, encontre e retorne a soma de todos os dígitos individuais presentes nela. (Ex: "a1b2c3" -> 6).

---

### **Gabarito Comentado**

#### **Resposta Teste 1: Cifra de César Simples**

```java
public class CifraCesar {
    public static String resolve(String texto, int deslocamento) {
        // StringBuilder é ideal para construir a nova string caractere por caractere.
        StringBuilder resultado = new StringBuilder();
        
        // Normaliza o deslocamento para o intervalo do alfabeto (0-25)
        deslocamento = deslocamento % 26;

        for (int i = 0; i < texto.length(); i++) {
            char c = texto.charAt(i);

            // Verifica se o caractere é uma letra minúscula
            if (c >= 'a' && c <= 'z') {
                char novoChar = (char) (c + deslocamento);
                // Lida com o "wrap-around" (ex: 'z' + 2 -> 'b')
                if (novoChar > 'z') {
                    novoChar = (char) (novoChar - 26);
                }
                resultado.append(novoChar);
            } 
            // Verifica se é uma letra maiúscula
            else if (c >= 'A' && c <= 'Z') {
                char novoChar = (char) (c + deslocamento);
                if (novoChar > 'Z') {
                    novoChar = (char) (novoChar - 26);
                }
                resultado.append(novoChar);
            } 
            // Se não for letra, apenas adiciona o caractere original
            else {
                resultado.append(c);
            }
        }
        return resultado.toString();
    }
}
```

#### **Resposta Teste 2: Par com Menor Diferença**

```java
import java.util.Arrays;

public class ParMenorDiferenca {
    public static int[] resolve(int[] nums, int alvo) {
        // Ordena o array para permitir uma busca eficiente com dois ponteiros.
        Arrays.sort(nums);
        int[] parResposta = new int[2];
        int menorDiferenca = Integer.MAX_VALUE;

        int esquerda = 0;
        int direita = nums.length - 1;

        // Técnica dos dois ponteiros: um no início, um no fim.
        while (esquerda < direita) {
            int soma = nums[esquerda] + nums[direita];
            int diferencaAtual = Math.abs(nums[esquerda] - nums[direita]);

            if (soma == alvo) {
                // Se a soma for a alvo, verificamos se a diferença é a menor.
                if (diferencaAtual < menorDiferenca) {
                    menorDiferenca = diferencaAtual;
                    parResposta[0] = nums[esquerda];
                    parResposta[1] = nums[direita];
                }
                // Mesmo encontrando, continuamos a busca para ver se há um par com diferença menor.
                // Movemos o ponteiro da direita para tentar diminuir a diferença.
                direita--; 
            } else if (soma < alvo) {
                // Se a soma é menor que o alvo, precisamos aumentar. Movemos o ponteiro da esquerda.
                esquerda++;
            } else { // soma > alvo
                // Se a soma é maior, precisamos diminuir. Movemos o ponteiro da direita.
                direita--;
            }
        }
        return parResposta;
    }
}
```

#### **Resposta Teste 3: Palavra Mais Frequente**

```java
import java.util.HashMap;
import java.util.Map;

public class PalavraFrequente {
    public static String resolve(String frase) {
        if (frase == null || frase.trim().isEmpty()) {
            return "";
        }

        // HashMap é perfeito para contar frequências: <Palavra, Quantidade>
        Map<String, Integer> frequencias = new HashMap<>();
        String[] palavras = frase.toLowerCase().split("\\s+"); // Divide por um ou mais espaços

        for (String palavra : palavras) {
            // Limpa a palavra de possíveis pontuações (opcional, mas bom)
            palavra = palavra.replaceAll("[^a-zA-Z]", "");
            if (!palavra.isEmpty()) {
                // getOrDefault pega a contagem atual ou 0 se for a primeira vez.
                frequencias.put(palavra, frequencias.getOrDefault(palavra, 0) + 1);
            }
        }

        String palavraMaisFrequente = "";
        int maxContagem = 0;

        // Percorre o mapa para encontrar a entrada com o maior valor.
        for (Map.Entry<String, Integer> entry : frequencias.entrySet()) {
            if (entry.getValue() > maxContagem) {
                maxContagem = entry.getValue();
                palavraMaisFrequente = entry.getKey();
            }
        }

        return palavraMaisFrequente;
    }
}
```

#### **Resposta Teste 4: Número Palíndromo**

```java
public class NumeroPalindromo {
    public static boolean resolve(int numero) {
        // Números negativos não são palíndromos.
        if (numero < 0) {
            return false;
        }
        
        // A abordagem mais simples é converter o número para String.
        String numeroStr = Integer.toString(numero);
        int esquerda = 0;
        int direita = numeroStr.length() - 1;

        // Compara os caracteres de fora para dentro.
        while (esquerda < direita) {
            if (numeroStr.charAt(esquerda) != numeroStr.charAt(direita)) {
                return false; // Se encontrar um par diferente, não é palíndromo.
            }
            esquerda++;
            direita--;
        }
        return true; // Se o laço terminar, é palíndromo.
    }
}
```

#### **Resposta Teste 5: Inverter Palavras da Frase**

```java
public class InverterPalavras {
    public static String resolve(String frase) {
        if (frase == null || frase.trim().isEmpty()) {
            return "";
        }
        
        // 1. Divide a frase em um array de palavras.
        String[] palavras = frase.split(" ");
        
        // 2. Usa StringBuilder para construir a frase invertida.
        StringBuilder resultado = new StringBuilder();
        
        // 3. Percorre o array de trás para frente.
        for (int i = palavras.length - 1; i >= 0; i--) {
            resultado.append(palavras[i]);
            // Adiciona um espaço, mas não após a última palavra.
            if (i > 0) {
                resultado.append(" ");
            }
        }
        
        return resultado.toString();
    }
}
```

#### **Resposta Teste 6: Soma de Preços com Stream**

```java
import java.util.List;
import java.util.stream.Collectors;

// Classe de suporte para o teste
class Produto {
    String nome;
    double preco;
    Produto(String nome, double preco) { this.nome = nome; this.preco = preco; }
    public double getPreco() { return preco; }
    public String getNome() { return nome; }
}

public class SomaPrecosStream {
    public static double resolve(List<Produto> produtos) {
        // A pipeline do stream resolve o problema de forma declarativa.
        return produtos.stream()
            // Filtra a lista, mantendo apenas os produtos cujo nome começa com "A"
            .filter(p -> p.getNome().startsWith("A"))
            // Mapeia o stream de Produto para um stream de double (os preços)
            .mapToDouble(Produto::getPreco)
            // Operação terminal: soma todos os elementos do stream de double
            .sum();
    }
}
```

#### **Resposta Teste 7: Segundo Maior Número**

```java
public class SegundoMaior {
    public static int resolve(int[] nums) {
        if (nums == null || nums.length < 2) {
            throw new IllegalArgumentException("Array precisa ter pelo menos dois elementos.");
        }

        int maior = Integer.MIN_VALUE;
        int segundoMaior = Integer.MIN_VALUE;

        for (int num : nums) {
            if (num > maior) {
                // Se o número atual for maior que o 'maior', o antigo 'maior' se torna o 'segundoMaior'
                segundoMaior = maior;
                maior = num;
            } else if (num > segundoMaior && num != maior) {
                // Se não for o maior, mas for maior que o 'segundoMaior', atualiza o 'segundoMaior'
                segundoMaior = num;
            }
        }
        
        // Se segundoMaior continuou como MIN_VALUE, pode ser que todos os números fossem iguais.
        // Nesse caso, não há um segundo maior distinto.
        return (segundoMaior == Integer.MIN_VALUE) ? maior : segundoMaior;
    }
}
```

#### **Resposta Teste 8: Verificar Anagrama**

```java
import java.util.Arrays;

public class VerificaAnagrama {
    public static boolean resolve(String str1, String str2) {
        // Anagramas devem ter o mesmo comprimento.
        if (str1.length() != str2.length()) {
            return false;
        }

        // A forma mais simples: limpar as strings, converter para minúsculas,
        // transformar em array de caracteres e ordenar.
        char[] chars1 = str1.toLowerCase().toCharArray();
        char[] chars2 = str2.toLowerCase().toCharArray();

        Arrays.sort(chars1);
        Arrays.sort(chars2);

        // Se os arrays ordenados forem idênticos, são anagramas.
        return Arrays.equals(chars1, chars2);
    }
}
```

#### **Resposta Teste 9: Imprimir Padrão de Pirâmide**

```java
public class PiramideAsteriscos {
    public static void resolve(int n) {
        // Laço externo para cada andar da pirâmide.
        for (int i = 1; i <= n; i++) {
            // Laço interno para imprimir os espaços em branco antes dos asteriscos.
            // A quantidade de espaços é (n - i).
            for (int j = 0; j < n - i; j++) {
                System.out.print(" ");
            }
            // Laço interno para imprimir os asteriscos.
            // A quantidade de asteriscos é (2 * i - 1).
            for (int k = 0; k < 2 * i - 1; k++) {
                System.out.print("*");
            }
            // Pula para a próxima linha após imprimir o andar.
            System.out.println();
        }
    }
}
```

#### **Resposta Teste 10: Soma dos Dígitos em uma String**

```java
public class SomaDigitosString {
    public static int resolve(String str) {
        int soma = 0;
        // Percorre cada caractere da string.
        for (int i = 0; i < str.length(); i++) {
            char c = str.charAt(i);
            // Verifica se o caractere é um dígito usando o método da classe Character.
            if (Character.isDigit(c)) {
                // Converte o caractere dígito para seu valor numérico inteiro.
                // '5' (char) -> 5 (int)
                soma += c - '0'; 
            }
        }
        return soma;
    }
}
```
