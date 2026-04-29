# Trabalho de Administração de Redes
## Protocolo SNMP

---

## 1. O Papel do SNMP

O SNMP (Simple Network Management Protocol) é um protocolo da camada de aplicação utilizado para o gerenciamento de redes de computadores. Sua principal finalidade é permitir o monitoramento, a coleta de informações e o controle de dispositivos de rede, como roteadores, switches e servidores.

Por meio do SNMP, administradores conseguem acompanhar o desempenho da rede, identificar falhas e, em alguns casos, realizar configurações remotas. Esse processo ocorre por meio da troca de mensagens entre um sistema central de gerenciamento e os dispositivos monitorados.

A interoperabilidade é um aspecto fundamental do SNMP, pois redes corporativas são compostas por equipamentos de diferentes fabricantes. A utilização de um protocolo padronizado garante que todos esses dispositivos possam ser gerenciados de forma unificada, evitando a necessidade de múltiplas ferramentas proprietárias e reduzindo a complexidade da administração da rede.

---

## 2. Evolução e Versões (v1, v2c e v3)

O SNMP passou por diversas evoluções com o objetivo de melhorar sua eficiência e segurança.

### Segurança
- **SNMPv1:** Utiliza *community strings* em texto plano, sendo vulnerável.
- **SNMPv2c:** Mantém o mesmo modelo de segurança da versão anterior.
- **SNMPv3:** Introduz autenticação, criptografia e controle de acesso.

### Desempenho
- **SNMPv1:** Limitado para grandes volumes de dados.
- **SNMPv2c:** Introduz o comando GETBULK, melhorando a eficiência.
- **SNMPv3:** Mantém as melhorias, com pequeno overhead de segurança.

### Padrão Atual
O SNMPv3 é a versão mais recomendada para ambientes corporativos, pois oferece maior segurança e confiabilidade, sendo adequado para redes modernas.

---

## 3. Arquitetura e Funcionamento

Um sistema SNMP é composto por três elementos principais:

### Gerente (NMS - Network Management Station)
Responsável por:
- Enviar requisições
- Receber respostas
- Monitorar e analisar a rede

### Agente (Agent)
- Reside nos dispositivos de rede
- Coleta informações locais
- Responde ao gerente
- Envia notificações (TRAPs)

### MIB (Management Information Base)
- Banco de dados hierárquico
- Armazena informações gerenciáveis do dispositivo

### OID (Object Identifier)
- Identificador único de cada variável
- Representado por sequência numérica

---

## 4. Ecossistema de Softwares

Alguns softwares utilizados para monitoramento via SNMP:

- Zabbix  
- PRTG Network Monitor  
- Nagios  

Essas ferramentas permitem visualizar dados em forma de gráficos, gerar alertas e relatórios, auxiliando na administração da rede.

---

## Referencias

KUROSE, James F.; ROSS, Keith W. Computer Networking: A Top-Down Approach. 7. ed. Pearson, 2017.

OPENAI. ChatGPT (modelo GPT-5.3). Utilizado como ferramenta de apoio para explicações e organização do conteúdo. Disponível em: https://chat.openai.com
. Acesso em: 29 abr. 2026.
