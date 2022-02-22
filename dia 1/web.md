# TCP/IP, portas, roteadores, switches e modems

Protocolos de comunicação entre computadores em rede.

- Transmission Control Protocol - Protocolo de Controle de Transmissão
- Internet Protocol - Protocolo de Internet
- ↑ Usam modelo de camadas:
    1. Física (placa de rede)
    2. Rede (IP)
    3. Transporte (TCP, UDP)
        - Os dois ja estão configurados no computador.
        - UDP
            - Rápido
            - Não confiável (coisas podem se perder no caminho)
            - Livestram
        - TCP
            - Voltando à conexão
            - Handshake (todo mundo sabe quem, pq e oq esta sendo mandado)
            - Integridade, ordem dos dados
            - Aplicativo de mensagens de texto
    4. Aplicação (FTP, SMTP, HTTP)

---

- Portas (Ports)
    - “Portinhas” por onde dados siarão e chegarão.
        - 20: FTP
        - 22: SSH
        - 25: SMTP
        - 53: DNS
        - 80: HTTP
        - 443: HTTPS

> Modem: *Mo*dulator-*dem*odulator. É um Hardware que converte dados em um formato que possa ser transmitido de um computador para outro e lido por outro.
> 

Roteador: distribui internet para um ou mais dispositivos de um rede. 

- Pode fazer a comunicação entre redes.
- Pode ser “burro” (hoje em dia ja são mais “inteligentes”)

Switch: distribui internet para um ou mais dispositivos de um rede. 

- Criado para ser “inteligente”
