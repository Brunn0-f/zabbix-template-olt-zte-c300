# 📡 Zabbix Template - OLT ZTE C300

Template completo de monitoramento para **OLT ZTE C300** no Zabbix.

---

## 📋 Descrição

Este template foi criado para fornecer um monitoramento detalhado de OLTs ZTE C300, utilizando descobertas automáticas e triggers avançadas.  
Ele foi projetado para ambientes ISP e redes FTTH, permitindo uma visão completa do estado operacional das OLTs.

---

## 🚀 Funcionalidades

### Itens Monitorados

- **Temperatura da OLT**
- **Uptime da OLT**
- **Temperatura das Placas**
- **Uso de CPU por placa**
- **Uso de Memória por placa**
- **Status das Placas**
- **Status das Interfaces Ethernet**
- **Rotação das Fans**
- **Sinal Óptico (Atenuação)**
- **Quantidade de ONUs Online**

### Descobertas Automáticas (LLD)

| Descoberta                      | Recursos Monitorados                                      |
|---------------------------------|----------------------------------------------------------|
| `Rotação Fans`                  | Estado e rotação das fans                                |
| `Status Placas`                 | Temperatura, CPU, memória e status das placas            |
| `Descobertas de Sinal`          | Atenuação das interfaces GPON                            |
| `Descobertas de CPU`            | Uso de CPU por placa                                     |
| `Descobertas de Interfaces`     | Status de links de interfaces                           |
| `Descobertas Ethernet 64Bits`   | Tráfego de bits em interfaces Ethernet                   |
| `Descobertas de GPON`           | ONUs autorizadas e online                               |
| `Descobertas de Memória`        | Uso de memória por placa                                 |

### Triggers Avançadas

- Temperatura acima do limite
- Reinício da OLT detectado
- Degradação de sinal óptico
- Uso elevado de CPU e Memória
- FAN parada ou rotação anormal
- Placa offline
- Link de interface PON offline
- Quedas massivas de ONUs

### Gráficos

- Gráficos automáticos via protótipos LLD, incluindo:
  - Temperatura
  - Uso de CPU
  - Uso de Memória
  - Rotação das Fans
  - Tráfego de interfaces Ethernet
  - Atenuação óptica

---

## 🛠️ Requisitos

- Zabbix Server com suporte SNMP (versão compatível)
- SNMPv2 ou SNMPv3 configurado na OLT
- OIDs compatíveis com modelo ZTE C300
- Importação do arquivo `zbx_export_templates.yaml` no Zabbix

---

## ⚙️ Instalação

1. Clone este repositório:
    ```bash
    git clone https://github.com/Brunn0-f/zabbix-template-olt-zte-c300b.git
    ```

2. Importe o template no Zabbix:
    - Navegue até **Configuration > Templates > Import**  
    - Selecione o arquivo `zbx_export_templates.yaml`  
    - Confirme a importação.

3. Associe o template a um host configurado com SNMP.

---

## 📝 Licença

MIT License

---

## 🙋‍♂️ Autor

Criado por **Bruno França**  
Data: 28/02/2025

---

