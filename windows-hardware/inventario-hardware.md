# Laboratório 01 — Inventário de Hardware

## 1. Objetivo

Identificar os principais componentes de hardware de um computador e coletar suas especificações utilizando ferramentas nativas do Windows.

## 2. Ambiente utilizado

- Sistema operacional: Windows 11
- Ferramentas: Gerenciador de Tarefas, Informações do Sistema (`msinfo32`) e PowerShell.

## 3. Configuração identificada

| Componente | Especificação |
|---|---|
| Processador | AMD Ryzen 7 9700X |
| Núcleos / Threads | 8 / 16 |
| Memória RAM | 32 GB DDR5 |
| Velocidade da memória | 6000 MT/s |
| Placa-mãe | Gigabyte B650M D3HP |
| Placa de vídeo | NVIDIA GeForce RTX 4060 |
| Armazenamento | Kingston NV3 1 TB NVMe |
| Firmware | UEFI |

## 4. Ferramentas e procedimentos

### Gerenciador de Tarefas

Acessado por `Ctrl + Shift + Esc`, na aba Desempenho, para identificar processador, memória, GPU e armazenamento.

### Informações do Sistema

Executado pelo comando:

```powershell
msinfo32
```

Permitiu consultar informações do sistema operacional, processador, memória e placa-mãe.

## 5. Comandos PowerShell utilizados

### Identificação da memória RAM

```powershell
Get-CimInstance Win32_PhysicalMemory |
Format-Table DeviceLocator, Capacity, Speed, ConfiguredClockSpeed, Manufacturer, PartNumber
```

### Identificação dos dispositivos de armazenamento

```powershell
Get-PhysicalDisk |
Format-Table FriendlyName, MediaType, BusType, Size, HealthStatus
```

## 6. Resultados e aprendizado

O laboratório permitiu identificar os principais componentes do computador e compreender como coletar informações técnicas utilizando ferramentas nativas do Windows e PowerShell.

## 7. Competências praticadas

- Inventário de hardware.
- Identificação de componentes.
- Utilização do Gerenciador de Tarefas.
- Consulta de informações do sistema.
- Coleta de dados via PowerShell.
