# Laboratório 03 — Diagnóstico de Armazenamento

## 1. Objetivo

Consultar indicadores de confiabilidade do SSD utilizando PowerShell e compreender informações relacionadas à temperatura, desgaste e possíveis erros de armazenamento.

## 2. Ambiente utilizado

- Sistema operacional: Windows 11
- Armazenamento: Kingston NV3 1 TB NVMe
- Ferramenta: Windows PowerShell

## 3. Comando utilizado

```powershell
Get-PhysicalDisk | Get-StorageReliabilityCounter | Format-List *
```

## 4. Resultados observados

| Indicador | Resultado |
|---|---|
| Temperatura | 34 °C |
| Wear | 0 |
| TemperatureMax | 75 |
| HealthStatus | Healthy |
| Campos de erros | Sem valores reportados |

## 5. Interpretação técnica

O comando permite consultar indicadores de confiabilidade disponibilizados pelo dispositivo de armazenamento.

O campo Wear apresentou valor 0 e o estado reportado pelo Windows foi Healthy.

Os campos de erros não apresentaram valores. Portanto, não é possível concluir que todos os contadores de erros sejam zero.

O resultado representa as informações disponibilizadas pelo dispositivo no momento da consulta e não garante ausência de qualquer falha.

## 6. Aprendizados

- Consultar indicadores de confiabilidade de SSDs.
- Identificar informações de temperatura e desgaste.
- Interpretar o estado de integridade reportado pelo Windows.
- Evitar conclusões sem evidências suficientes.

## 7. Competências praticadas

- Diagnóstico inicial de armazenamento.
- PowerShell.
- Interpretação de indicadores de hardware.
- Troubleshooting de dispositivos de armazenamento.
