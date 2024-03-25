# Exemplos de uso do comando ``tcpdump`

1. **Capturar todos os pacotes em uma interface de rede específica:**
   ```
   tcpdump -i eth0
   ```

2. **Capturar pacotes em uma interface de rede e salvar em um arquivo para análise posterior:**
   ```
   tcpdump -i eth0 -w output.pcap
   ```

3. **Exibir pacotes com informações detalhadas de cabeçalho IP e TCP:**
   ```
   tcpdump -i eth0 -vv
   ```

4. **Filtrar pacotes com base em um endereço IP de origem específico:**
   ```
   tcpdump src 192.168.1.100
   ```

5. **Filtrar pacotes com base em um endereço IP de destino específico:**
   ```
   tcpdump dst 192.168.1.200
   ```

6. **Filtrar pacotes com base em uma porta de origem específica:**
   ```
   tcpdump src port 80
   ```

7. **Filtrar pacotes com base em uma porta de destino específica:**
   ```
   tcpdump dst port 443
   ```

8. **Filtrar pacotes com base em um protocolo específico (por exemplo, ICMP):**
   ```
   tcpdump icmp
   ```

9. **Filtrar pacotes com base em um intervalo de endereços IP:**
   ```
   tcpdump net 192.168.1.0/24
   ```

10. **Filtrar pacotes com base em uma expressão complexa usando operadores lógicos:**
    ```
    tcpdump 'src host 192.168.1.100 and dst port 22'
    ```

11. **Capturar pacotes IPv6 em uma interface específica:**
    ```
    tcpdump -i eth0 ip6
    ```

12. **Exibir apenas os payloads dos pacotes (dados úteis):**
    ```
    tcpdump -i eth0 -s 0 -A
    ```

13. **Capturar pacotes ARP (Address Resolution Protocol):**
    ```
    tcpdump arp
    ```

14. **Exibir apenas pacotes que contenham dados maiores que um certo tamanho (bytes):**
    ```
    tcpdump greater 1000
    ```

15. **Capturar pacotes que correspondam a um padrão específico usando expressões regulares:**
    ```
    tcpdump -i eth0 'tcp[tcpflags] & (tcp-syn|tcp-fin) != 0'
    ```

16. **Capturar pacotes com base em um determinado número de pacotes ou duração de captura:**
    ```
    tcpdump -i eth0 -c 1000
    tcpdump -i eth0 -G 3600 -W 5
    ```

17. **Capturar pacotes com base em uma sequência de bytes específica (hexadecimal):**
    ```
    tcpdump -i eth0 'tcp[((tcp[12:1] & 0xf0) >> 2):4] = 0x47455420'
    ```

18. **Capturar e exibir pacotes usando um formato específico para a saída:**
    ```
    tcpdump -i eth0 -nn -tttt -r arquivo.pcap
    ```

19. **Capturar pacotes e exibir informações de cabeçalho em formato hexadecimal:**
    ```
    tcpdump -i eth0 -xx
    ```

20. **Usar um filtro BPF (Berkley Packet Filter) personalizado para captura:**
    ```
    tcpdump -i eth0 'tcp and port 80'
    ```
