# Laboratório 02 — Identificação de Hardware via PowerShell

## 1. Objetivo

Utilizar comandos PowerShell para identificar características da memória RAM e dos dispositivos de armazenamento.

## 2. Identificação da memória RAM

### Comando utilizado

```powershell
Get-CimInstance Win32_PhysicalMemory | Format-Table DeviceLocator, Capacity, Speed, ConfiguredClockSpeed, Manufacturer, PartNumber
```

### Resultados obtidos

- Quantidade de módulos: 2
- Capacidade por módulo: 16 GB
- Capacidade total: 32 GB
- Velocidade: 6000 MT/s
- Velocidade configurada: 6000 MT/s
- Fabricante: A-DATA Technology
- Part Number: AX5U6000C3016G-DCLARBK

## 3. Identificação do armazenamento

### Comando utilizado

```powershell
Get-PhysicalDisk | Format-Table FriendlyName, MediaType, BusType, Size, HealthStatus
```

### Resultados obtidos

- Modelo: Kingston SNV3S1000G
- Tipo: SSD
- Interface: NVMe
- Capacidade: aproximadamente 1 TB
- Estado reportado: Healthy

## 4. Interpretação técnica

O PowerShell permitiu identificar os módulos de memória instalados, suas capacidades e velocidades, além de consultar informações do SSD.

O campo HealthStatus apresentou o estado Healthy, indicando que o Windows reportou o dispositivo como saudável no momento da consulta.

## 5. Competências praticadas

- Utilização de cmdlets PowerShell.
- Consulta de informações via WMI/CIM.
- Identificação de memória RAM.
- Identificação de dispositivos de armazenamento.
- Interpretação de resultados técnicos.
