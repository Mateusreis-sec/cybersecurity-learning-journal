# TCP/IP — Fundamentos de Redes

## 1. O que é TCP/IP?

TCP/IP é o conjunto de protocolos utilizado para permitir a comunicação entre dispositivos em uma rede, incluindo a internet.

Ele define como os dados são endereçados, transportados e encaminhados entre a origem e o destino.

## 2. Modelo TCP/IP

O modelo TCP/IP pode ser representado em quatro camadas:

| Camada | Função | Exemplos |
|---|---|---|
| Aplicação | Oferece protocolos utilizados pelas aplicações | HTTP, HTTPS, DNS |
| Transporte | Organiza a comunicação entre aplicações | TCP, UDP |
| Internet | Trata do endereçamento IP e do encaminhamento entre redes | IPv4, IPv6, ICMP |
| Acesso à rede | Trata da comunicação na rede local e do envio de quadros | Ethernet, Wi-Fi |

## 3. Como os dados são transmitidos?

Quando um computador acessa um site, os dados passam pelas camadas do modelo TCP/IP.

1. A aplicação prepara os dados, por exemplo, uma requisição HTTP.
2. A camada de transporte utiliza TCP ou UDP, conforme o protocolo e a comunicação necessária.
3. A camada Internet utiliza IP para endereçar os pacotes e permitir seu encaminhamento.
4. A camada de acesso à rede transmite os quadros pelo meio físico ou sem fio.

No destino, o processo acontece de forma inversa até que a aplicação receba os dados.

Esse processo é chamado de encapsulamento.

## 4. TCP e UDP

**TCP (Transmission Control Protocol)** oferece uma comunicação orientada à conexão, com mecanismos para entrega confiável, ordenação dos dados e retransmissão quando necessário.

**UDP (User Datagram Protocol)** envia datagramas sem estabelecer uma conexão TCP e não garante, por si só, entrega ou ordenação.

A escolha depende das necessidades da aplicação.

## 5. Endereços IP e MAC

O endereço IP é utilizado para identificar a origem e o destino na comunicação IP.

O endereço MAC é utilizado na entrega de quadros dentro de um enlace de rede, como uma rede Ethernet.

Quando um pacote precisa atravessar roteadores, os endereços IP de origem e destino normalmente permanecem os mesmos ao longo do caminho, enquanto os endereços MAC do quadro são substituídos a cada enlace. Existem exceções, como mudanças causadas por NAT.

## 6. Relação com segurança

Compreender TCP/IP ajuda a:

- Interpretar conexões e tráfego de rede.
- Analisar capturas no Wireshark.
- Entender portas, protocolos e serviços.
- Investigar comunicações suspeitas durante uma análise de SOC.

## 7. Status do estudo

- [x] Estudo introdutório do modelo TCP/IP.
- [ ] Revisar o encapsulamento na prática.
- [ ] Analisar uma comunicação com o Wireshark.

## 8. Referências

- [RFC 9293 — Transmission Control Protocol (TCP)](https://www.rfc-editor.org/rfc/rfc9293)
- [RFC 768 — User Datagram Protocol (UDP)](https://www.rfc-editor.org/rfc/rfc768)
