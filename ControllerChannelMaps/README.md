# ControllerChannelMap

Esta pasta contém dados de mapeamento de canais do controlador de motor capturados via VCDS para a ECU ME17.5.24 utilizada nos veículos Novo Gol, Fox, Voyage a partir de 2013.

## Arquivos

### `01-030-906-020-E-20240914-1816.PLB`

Arquivo de **Live Data (PLB)** capturado em **14 de Setembro de 2024 às 18:16:20**.

**Características:**
- Formato de dados brutos do VCDS
- Contém medições em tempo real de sensores do motor
- Mapeia 4 canais principais com dados automotivos:
  - **Canal 1:** RPM (~840 /min), Temperatura (~73°C), Lambda (~0.4%), Bits binários
  - **Canal 2:** RPM (~840 /min), Carga (~19.5%), Tempo (~2.04 ms), Pressão absoluta (~320 mbar)
  - **Canal 3:** RPM (~840 /min), Pressão (~320 mbar), Carga (~3.1%), Avanço de ignição (~3.8° BTDC)
  - **Canal 4:** RPM (~840 /min), Tensão (~13.912 V), Temperatura motor (~73°C), Temperatura (~32°C)

- **ECU:** ME17.5.24 com Coding: 1C02108E100F4010
- **Hardware:** 030-907-309-A (Engine Control Unit)
- **Software:** 030-906-020-E
- **VCDS Version:** Release 24.5.0

### `01-030-906-020-E-20240914-1817.PLA`

Arquivo de **Live Data em formato Alfanumérico (PLA)** capturado em **14 de Setembro de 2024 às 18:17:39**.

**Características:**
- Formato mais legível com labels dos canais
- Contém os mesmos dados parametrizados com nomes descritivos
- Mapeia canais com identificadores (A01, A07, A13, etc.):
  - **A01:** Valores numéricas (128), RPM (~850 /min), Estado do A/C (Compressor OFF)
  - **A07:** Detecta erros e aviso de segurança/acesso
  - **A13:** Valores booleanas (0/N/A)

- **Mesmos metadados de ECU e Hardware que o arquivo PLB**

## Diferenças entre os Formatos

| Aspecto | PLB | PLA |
|--------|-----|-----|
| **Formato** | Numérico estruturado | Alfanumérico com labels |
| **Legibilidade** | Menor | Maior |
| **Uso** | Processamento automático, ferramentas especializadas | Análise manual, documentação |
| **Intervalo de captura** | 1 minuto de diferença | - |

## ECU Mapeado

- **Software (SW):** 030-906-020-E
- **Hardware (HW):** 030-907-309-A (Engine Control Module)
- **Componente:** ME17.5.24 (Motronic Engine System)
- **Coding:** 1C02108E100F4010

Estes arquivos servem para análise de performance do motor e diagnóstico através do sistema VCDS.
