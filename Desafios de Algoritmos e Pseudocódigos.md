# Desafios de Algoritmos e Pseudocódigos

## Desafios Iniciais

1. **Soma de Dois Números**
   - **Descrição:** Crie um algoritmo que solicite ao usuário dois números e exiba a soma deles.
   - **Pseudocódigo:**
     ```
     ALGORITMO Soma_Dois_Numeros
       INÍCIO
         Solicitar ao usuário o primeiro número e armazenar em 'num1'
         Solicitar ao usuário o segundo número e armazenar em 'num2'
         Calcular a soma de 'num1' e 'num2' e armazenar em 'soma'
         Exibir 'soma'
       FIM
     ```

2. **Verificação de Par ou Ímpar**
   - **Descrição:** Crie um algoritmo que verifique se um número fornecido pelo usuário é par ou ímpar.
   - **Pseudocódigo:**
     ```
     ALGORITMO Verificar_Par_ou_Impar
       INÍCIO
         Solicitar ao usuário um número e armazenar em 'numero'
         SE 'numero' % 2 == 0 ENTÃO
           Exibir "O número é par"
         SENÃO
           Exibir "O número é ímpar"
         FIM_SE
       FIM
     ```

3. **Maior de Três Números**
   - **Descrição:** Crie um algoritmo que determine o maior entre três números fornecidos pelo usuário.
   - **Pseudocódigo:**
     ```
     ALGORITMO Maior_de_Tres_Numeros
       INÍCIO
         Solicitar ao usuário três números e armazenar em 'num1', 'num2' e 'num3'
         SE 'num1' >= 'num2' E 'num1' >= 'num3' ENTÃO
           Exibir 'num1' é o maior
         SENÃO SE 'num2' >= 'num1' E 'num2' >= 'num3' ENTÃO
           Exibir 'num2' é o maior
         SENÃO
           Exibir 'num3' é o maior
         FIM_SE
       FIM
     ```

## Desafios Intermediários

4. **Cálculo de Média**
   - **Descrição:** Crie um algoritmo que calcule a média de quatro notas fornecidas pelo usuário.
   - **Pseudocódigo:**
     ```
     ALGORITMO Calcular_Media
       INÍCIO
         Solicitar ao usuário quatro notas e armazenar em 'nota1', 'nota2', 'nota3' e 'nota4'
         Calcular a média das notas e armazenar em 'media'
         Exibir 'media'
       FIM
     ```

5. **Fatorial de um Número**
   - **Descrição:** Crie um algoritmo que calcule o fatorial de um número fornecido pelo usuário.
   - **Pseudocódigo:**
     ```
     ALGORITMO Calcular_Fatorial
       INÍCIO
         Solicitar ao usuário um número e armazenar em 'numero'
         Inicializar 'fatorial' como 1
         PARA i DE 1 ATÉ 'numero' FAÇA
           'fatorial' = 'fatorial' * i
         FIM_PARA
         Exibir 'fatorial'
       FIM
     ```

6. **Contagem de Vogais**
   - **Descrição:** Crie um algoritmo que conte o número de vogais em uma string fornecida pelo usuário.
   - **Pseudocódigo:**
     ```
     ALGORITMO Contar_Vogais
       INÍCIO
         Solicitar ao usuário uma string e armazenar em 'texto'
         Inicializar 'contagem_vogais' como 0
         PARA cada caractere em 'texto' FAÇA
           SE caractere for uma vogal ENTÃO
             Incrementar 'contagem_vogais'
           FIM_SE
         FIM_PARA
         Exibir 'contagem_vogais'
       FIM
     ```

## Desafios Avançados

7. **Ordenação de Lista**
   - **Descrição:** Crie um algoritmo que ordene uma lista de números fornecida pelo usuário em ordem crescente.
   - **Pseudocódigo:**
     ```
     ALGORITMO Ordenar_Lista
       INÍCIO
         Solicitar ao usuário uma lista de números e armazenar em 'lista'
         PARA i DE 0 ATÉ tamanho de 'lista' - 1 FAÇA
           PARA j DE 0 ATÉ tamanho de 'lista' - i - 1 FAÇA
             SE 'lista'[j] > 'lista'[j + 1] ENTÃO
               Trocar 'lista'[j] e 'lista'[j + 1]
             FIM_SE
           FIM_PARA
         FIM_PARA
         Exibir 'lista' ordenada
       FIM
     ```

8. **Busca Binária**
   - **Descrição:** Crie um algoritmo que implemente a busca binária em uma lista ordenada de números fornecida pelo usuário.
   - **Pseudocódigo:**
     ```
     ALGORITMO Busca_Binaria
       INÍCIO
         Solicitar ao usuário uma lista ordenada de números e armazenar em 'lista'
         Solicitar ao usuário o número a ser buscado e armazenar em 'numero'
         Inicializar 'inicio' como 0 e 'fim' como tamanho de 'lista' - 1
         ENQUANTO 'inicio' <= 'fim' FAÇA
           Calcular 'meio' como ('inicio' + 'fim') / 2
           SE 'lista'[meio] == 'numero' ENTÃO
             Exibir 'numero' encontrado na posição 'meio'
             Parar
           SENÃO SE 'lista'[meio] < 'numero' ENTÃO
             'inicio' = 'meio' + 1
           SENÃO
             'fim' = 'meio' - 1
           FIM_SE
         FIM_ENQUANTO
         SE 'numero' não foi encontrado ENTÃO
           Exibir 'numero' não encontrado
         FIM_SE
       FIM
     ```

9. **Verificação de Palíndromo**
   - **Descrição:** Crie um algoritmo que verifique se uma string fornecida pelo usuário é um palíndromo.
   - **Pseudocódigo:**
     ```
     ALGORITMO Verificar_Palindromo
       INÍCIO
         Solicitar ao usuário uma string e armazenar em 'texto'
         Inicializar 'texto_invertido' como ''
         PARA i DE tamanho de 'texto' - 1 ATÉ 0 FAÇA
           'texto_invertido' = 'texto_invertido' + 'texto'[i]
         FIM_PARA
         SE 'texto' == 'texto_invertido' ENTÃO
           Exibir 'texto' é um palíndromo
         SENÃO
           Exibir 'texto' não é um palíndromo
         FIM_SE
       FIM
     ```

10. **Cálculo de Números Primos**
    - **Descrição:** Crie um algoritmo que encontre todos os números primos até um número fornecido pelo usuário.
    - **Pseudocódigo:**
      ```
      ALGORITMO Encontrar_Primos
        INÍCIO
          Solicitar ao usuário um número e armazenar em 'limite'
          PARA n DE 2 ATÉ 'limite' FAÇA
            Inicializar 'eh_primo' como verdadeiro
            PARA i DE 2 ATÉ n - 1 FAÇA
              SE n % i == 0 ENTÃO
                'eh_primo' = falso
                Parar
              FIM_SE
            FIM_PARA
            SE 'eh_primo' ENTÃO
              Exibir n
            FIM_SE
          FIM_PARA
        FIM
      ```

Esses desafios são projetados para ajudar a praticar e consolidar os conceitos de algoritmos e pseudocódigos de forma progressiva. Boa prática!
