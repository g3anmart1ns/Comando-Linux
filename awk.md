## Exemplos de uso do comando AWK

```markdown
# Exemplos de Uso do Comando AWK

## Exibir o conteúdo de um arquivo:
```bash
awk '{print}' arquivo.txt
```

## Exibir a primeira coluna de um arquivo CSV:
```bash
awk -F ',' '{print $1}' arquivo.csv
```

## Exibir linhas que contêm uma determinada palavra:
```bash
awk '/palavra/' arquivo.txt
```

## Calcular a média de uma coluna numérica em um arquivo CSV:
```bash
awk -F ',' '{sum += $1} END {print "Média:", sum/NR}' arquivo.csv
```

## Contar o número de linhas em um arquivo:
```bash
awk 'END {print NR}' arquivo.txt
```

## Substituir uma string por outra em um arquivo:
```bash
awk '{gsub("string_antiga", "string_nova")}1' arquivo.txt
```

## Exibir apenas linhas com mais de 10 caracteres:
```bash
awk 'length($0) > 10' arquivo.txt
```

## Exibir a terceira coluna se a primeira coluna atender a uma condição:
```bash
awk '$1 > 10 {print $3}' arquivo.txt
```

## Exibir a última linha de um arquivo:
```bash
awk 'END {print}' arquivo.txt
```

## Exibir o número de palavras em cada linha:
```bash
awk '{print NF}' arquivo.txt
```

## Exibir linhas em que a segunda coluna é maior que 100:
```bash
awk '$2 > 100' arquivo.txt
```

## Exibir linhas em que a terceira coluna é igual a "valor":
```bash
awk '$3 == "valor"' arquivo.txt
```

## Calcular a soma de uma coluna numérica em um arquivo CSV:
```bash
awk -F ',' '{sum += $1} END {print "Soma:", sum}' arquivo.csv
```

## Exibir linhas em que a primeira coluna começa com "abc":
```bash
awk '$1 ~ /^abc/' arquivo.txt
```

## Exibir linhas em que a segunda coluna é diferente de "valor":
```bash
awk '$2 != "valor"' arquivo.txt
```

## Exibir linhas em que a segunda coluna contém um número entre 50 e 100:
```bash
awk '$2 >= 50 && $2 <= 100' arquivo.txt
```

## Calcular a média de uma coluna numérica condicionalmente em um arquivo CSV (apenas para valores maiores que 50):
```bash
awk -F ',' '$1 > 50 {sum += $1; count++} END {print "Média:", sum/count}' arquivo.csv
```

## Inverter a ordem das colunas em um arquivo CSV:
```bash
awk -F ',' '{print $NF, $(NF-1), ..., $1}' arquivo.csv
```

## Exibir apenas linhas pares (ou ímpares) de um arquivo:
```bash
awk 'NR%2 == 0' arquivo.txt  # para linhas pares
awk 'NR%2 != 0' arquivo.txt  # para linhas ímpares
```

## Exibir a segunda e quarta colunas de um arquivo CSV:
```bash
awk -F ',' '{print $2, $4}' arquivo.csv
```
```
