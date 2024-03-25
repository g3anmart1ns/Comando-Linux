```markdown
# Exemplos de Uso do Comando `nmap`

1. **Escanear um Host:**
```bash
nmap 192.168.1.1
```

2. **Escanear um Intervalo de IPs:**
```bash
nmap 192.168.1.1-50
```

3. **Escanear um Subnet:**
```bash
nmap 192.168.1.0/24
```

4. **Escanear um Host e Mostrar Serviços e Versões:**
```bash
nmap -A 192.168.1.1
```

5. **Escanear um Host em Modo Silencioso:**
```bash
nmap -sS 192.168.1.1
```

6. **Escanear um Host e Mostrar Portas Abertas:**
```bash
nmap -p- 192.168.1.1
```

7. **Escanear um Host e Realizar um Traceroute:**
```bash
nmap --traceroute 192.168.1.1
```

8. **Escanear um Host e Salvar a Saída em um Arquivo XML:**
```bash
nmap -oX scan.xml 192.168.1.1
```

9. **Escanear um Host Usando um Arquivo de Lista de IPs:**
```bash
nmap -iL hosts.txt
```

10. **Escanear um Host e Ignorar a Resolução DNS Reversa:**
```bash
nmap -n 192.168.1.1
```

11. **Escanear um Host e Mostrar Portas TCP e UDP Abertas:**
```bash
nmap -sU -sT 192.168.1.1
```

12. **Escanear um Host e Mostrar Informações Detalhadas de Versão:**
```bash
nmap -sV 192.168.1.1
```

13. **Escanear um Host e Mostrar Sistemas Operacionais Possíveis:**
```bash
nmap -O 192.168.1.1
```

14. **Escanear um Host e Mostrar Serviços HTTP, SMTP e DNS:**
```bash
nmap -p 80,25,53 192.168.1.1
```

15. **Escanear um Host e Mostrar Serviços Comuns:**
```bash
nmap --top-ports 10 192.168.1.1
```

16. **Escanear um Host e Mostrar Estatísticas do Escaneamento:**
```bash
nmap --stats-every 10s 192.168.1.1
```

17. **Escanear um Host e Mostrar Informações de Tempo Real do Escaneamento:**
```bash
nmap --packet-trace 192.168.1.1
```

18. **Escanear um Host e Mostrar Hosts Ativos na Rede Local:**
```bash
nmap -sP 192.168.1.0/24
```

19. **Escanear um Host e Realizar um Escaneamento Intensivo:**
```bash
nmap -T4 -A -v 192.168.1.1
```

20. **Escanear um Host e Realizar um Escaneamento Rápido:**
```bash
nmap -F 192.168.1.1
```
