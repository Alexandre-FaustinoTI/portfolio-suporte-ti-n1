# Laboratório 04 — Diagnóstico de Memória RAM

## 1. Objetivo

Executar o diagnóstico de memória do Windows para verificar possíveis erros na memória RAM instalada.

## 2. Ambiente utilizado

- Sistema operacional: Windows 11
- Ferramenta: Diagnóstico de Memória do Windows
- Visualizador de Eventos

## 3. Procedimento realizado

1. Abrir a janela Executar com `Win + R`.
2. Digitar `mdsched.exe`.
3. Selecionar a opção "Reiniciar agora e verificar se há problemas".
4. Aguardar a execução do diagnóstico durante a reinicialização.
5. Após o retorno ao Windows, abrir o Visualizador de Eventos.
6. Acessar Logs do Windows → Sistema.
7. Localizar o evento MemoryDiagnostics-Results.

## 4. Resultado encontrado

| Indicador | Resultado |
|---|---|
| Origem | MemoryDiagnostics-Results |
| ID do evento | 1201 |
| Resultado | Nenhum erro de memória detectado |

Mensagem apresentada:

"O Diagnóstico de Memória do Windows testou a memória do computador e não detectou erros."

## 5. Interpretação técnica

O teste não identificou erros na memória RAM durante a verificação realizada.

Esse resultado é positivo, mas não garante ausência de todos os possíveis problemas de memória.

É importante diferenciar defeitos físicos na RAM de insuficiência de capacidade para executar vários programas simultaneamente.

## 6. Aprendizados

- Executar o diagnóstico de memória do Windows.
- Consultar resultados no Visualizador de Eventos.
- Identificar a origem e o ID de um evento.
- Interpretar resultados de diagnóstico.
- Diferenciar integridade da memória de capacidade disponível.

## 7. Competências praticadas

- Diagnóstico de hardware.
- Windows 11.
- Visualizador de Eventos.
- Troubleshooting de memória RAM.
