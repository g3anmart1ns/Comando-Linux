
# Exemplos de Uso do Comando `sed`

## Exemplos de Uso do Comando `sed`:

1. **Substituir uma string em um arquivo e imprimir na tela:**
```bash
sed 's/antiga/nova/' arquivo.txt
```

2. **Substituir todas as ocorrências de uma string em um arquivo e salvar o resultado em um novo arquivo:**
```bash
sed 's/antiga/nova/g' arquivo_origem.txt > arquivo_destino.txt
```

3. **Excluir linhas que correspondem a um padrão em um arquivo e imprimir na tela:**
```bash
sed '/padrão/d' arquivo.txt
```

4. **Excluir linhas em branco de um arquivo e imprimir na tela:**
```bash
sed '/^$/d' arquivo.txt
```

5. **Adicionar texto no início de cada linha de um arquivo e imprimir na tela:**
```bash
sed 's/^/texto_a_adicionar /' arquivo.txt
```

6. **Excluir um intervalo de linhas de um arquivo e imprimir na tela:**
```bash
sed 'N,Md' arquivo.txt
```

7. **Substituir apenas a primeira ocorrência de uma string em cada linha e imprimir na tela:**
```bash
sed 's/antiga/nova/' arquivo.txt
```

8. **Substituir apenas a segunda ocorrência de uma string em cada linha e imprimir na tela:**
```bash
sed 's/antiga/nova/2' arquivo.txt
```

9. **Inserir uma linha antes de uma linha correspondente a um padrão e imprimir na tela:**
```bash
sed '/padrão/i nova_linha' arquivo.txt
```

10. **Inserir uma linha após uma linha correspondente a um padrão e imprimir na tela:**
```bash
sed '/padrão/a nova_linha' arquivo.txt
```

11. **Remover caracteres especiais de um arquivo e imprimir na tela:**
```bash
sed 's/[^[:print:]]//g' arquivo.txt
```

12. **Extrair linhas com números de telefone de um arquivo e imprimir na tela:**
```bash
sed -n '/[0-9]\{3\}-[0-9]\{3\}-[0-9]\{4\}/p' arquivo.txt
```

13. **Remover linhas duplicadas de um arquivo e imprimir na tela:**
```bash
sed '$!N; /^\(.*\)\n\1$/!P; D' arquivo.txt
```

14. **Substituir espaços em branco por tabulações em um arquivo e imprimir na tela:**
```bash
sed 's/ \+/\t/g' arquivo.txt
```

15. **Inverter a ordem das palavras em cada linha de um arquivo e imprimir na tela:**
```bash
sed 's/\(.*\) \(.*\)/\2 \1/' arquivo.txt
```

16. **Comentar todas as linhas de um arquivo e imprimir na tela:**
```bash
sed 's/^/# /' arquivo.txt
```

17. **Remover comentários de um arquivo e imprimir na tela:**
```bash
sed 's/#.*//' arquivo.txt
```

18. **Extrair a primeira palavra de cada linha de um arquivo e imprimir na tela:**
```bash
sed 's/^\([^ ]*\).*$/\1/' arquivo.txt
```

19. **Contar o número de caracteres em cada linha de um arquivo e imprimir na tela:**
```bash
sed 's/[^[:space:]]//g' arquivo.txt | wc -m
```

20. **Inserir texto no final de cada linha que corresponde a um padrão e imprimir na tela:**
```bash
sed '/padrão/s/$/ texto_a_adicionar/' arquivo.txt
```
