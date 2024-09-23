
Mudanças e Correções
1. Correção de Operações Matemáticas
Erro: Na versão original, as operações de multiplicação e divisão estavam incorretas. O código realizava adição no caso de multiplicação e subtração no caso de divisão.
Correção: As operações matemáticas foram corrigidas para:
Multiplicação (x): setCurrentNumber((firstNumber * lastNumber).toString())
Divisão (/): setCurrentNumber((firstNumber / lastNumber).toString())

2. Correção de Exclusão de Caracteres com "DEL"
Erro: O código original removia dois caracteres ao invés de um ao pressionar "DEL".
Correção: A função foi corrigida para remover o último caractere corretamente: setCurrentNumber(currentNumber.substring(0, (currentNumber.length - 1))).

3. Adição de Função Percentual (%)
Melhoria: Foi implementada a função de porcentagem, que divide o valor atual por 100.
Código: case '%': setCurrentNumber(currentNumber / 100)

4. Função de Inversão de Sinal (+/-)
Correção: A função de inversão de sinal foi adicionada, multiplicando o valor atual por -1.
Código: case '+/-': setCurrentNumber(currentNumber * -1)

5. Correção da Ordem dos Botões
Erro: A ordem dos botões 4, 5, 6 estava incorreta no mapeamento inicial.
Correção: A ordem dos botões foi ajustada corretamente: 4, 5, 6.

6. Estilização Melhorada
Mudanças na cor de fundo e botões: A estilização foi atualizada para proporcionar uma experiência visual mais moderna e agradável.
Background: O fundo do aplicativo foi alterado para um tom mais escuro (#060047).
Botões: Os botões agora têm cores contrastantes e melhor visualização (fundo #3A1078 e texto branco).

7. Correção de Nomes de Variáveis
Erro: O nome da variável fistNumber estava incorreto.
Correção: A variável foi renomeada corretamente para firstNumber.

8. Correção de Fechamento de Tags JSX
Erro: No código original, a tag <View> não estava sendo corretamente fechada na área de exibição do resultado.
Correção: A tag foi fechada corretamente, evitando problemas de renderização.

9. Refinamento de Estilos
Ajustes nas cores de texto e espaçamento para garantir melhor legibilidade e usabilidade.
Uso
Cálculos Básicos: Insira os números e operadores como faria em uma calculadora tradicional. O botão = realiza o cálculo.
Controle de Operações:
"LIMPAR": Limpa toda a operação atual.
"DEL": Apaga o último caractere digitado.
"+/-": Inverte o sinal do número atual.
"%": Converte o número atual em porcentagem.
