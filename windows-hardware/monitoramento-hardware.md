# Laboratório 05 — Monitoramento de CPU e GPU

## 1. Objetivo

Monitorar temperaturas e utilização do processador e da placa de vídeo utilizando o HWiNFO.

## 2. Ambiente utilizado

- Sistema operacional: Windows 11
- Processador: AMD Ryzen 7 9700X
- Placa de vídeo: NVIDIA GeForce RTX 4060
- Ferramenta: HWiNFO

## 3. Procedimento realizado

1. Abrir o HWiNFO.
2. Selecionar o modo Sensors-only.
3. Localizar os sensores relacionados à CPU e GPU.
4. Observar temperaturas e utilização durante o repouso.
5. Registrar os valores atuais e máximos apresentados.

## 4. Resultados observados

| Indicador | CPU | GPU |
|---|---:|---:|
| Temperatura atual | 49,6 °C | 43,2 °C |
| Temperatura máxima | 58,4 °C | 44,9 °C |
| Utilização atual | 2,5% | 1% |

Outros indicadores:

- GPU Hotspot: aproximadamente 50,7 °C.
- Memória RAM utilizada: aproximadamente 25,9%.
- Ventoinhas da GPU: 0 RPM.

## 5. Interpretação técnica

Durante o monitoramento em repouso, as temperaturas observadas não indicaram superaquecimento.

A GPU apresentou ventoinhas paradas, comportamento compatível com o recurso Zero RPM, presente em determinadas placas de vídeo.

É importante considerar que os valores foram coletados durante o repouso, não sendo suficientes para avaliar estabilidade ou comportamento térmico sob carga.

## 6. Aprendizados

- Identificar sensores de temperatura da CPU e GPU.
- Diferenciar temperatura atual de máxima registrada.
- Consultar utilização dos componentes.
- Identificar comportamento de ventoinhas em repouso.
- Interpretar dados de monitoramento sem tirar conclusões precipitadas.

## 7. Competências praticadas

- Monitoramento de hardware.
- HWiNFO.
- Análise de temperatura.
- Diagnóstico preventivo.
- Interpretação de sensores.
