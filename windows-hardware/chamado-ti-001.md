# Chamado TI-001 — Lentidão durante utilização de aplicações

## 1. Identificação do chamado

- Número: TI-001
- Tipo: Simulação educacional de atendimento
- Categoria: Desempenho / Hardware
- Sistema operacional: Windows 11
- Usuário: João (personagem fictício)
- Responsável: Suporte Técnico N1

## 2. Descrição do problema

O usuário relatou lentidão no computador após aproximadamente 10 a 15 minutos de utilização.

O problema ocorria principalmente durante o uso simultâneo do Excel, com várias planilhas abertas, e do navegador.

Também foram relatadas dificuldades para alternar entre janelas e lentidão na abertura de programas.

## 3. Investigação inicial

Foram realizadas as seguintes verificações:

- Consulta ao Visualizador de Eventos.
- Análise do evento DistributedCOM, ID 10016.
- Monitoramento de CPU, memória RAM e disco pelo Gerenciador de Tarefas.
- Investigação de atualizações recentes do Windows e instalação de um leitor de PDF.

O evento DistributedCOM encontrado não apresentou relação comprovada com a lentidão.

## 4. Monitoramento de desempenho

### Primeira verificação

| Recurso | Utilização |
|---|---:|
| CPU | 28% |
| Memória RAM | 87% |
| Disco | 12% |
| Rede | 2% |

### Segunda verificação

Durante a repetição da atividade:

| Recurso | Utilização |
|---|---:|
| CPU | 35% |
| Memória RAM | 94% |
| Disco | 18% |
| Rede | 3% |

## 5. Diagnóstico de memória RAM

Foi executado o Diagnóstico de Memória do Windows utilizando:

```powershell
mdsched.exe
```

Resultado consultado no Visualizador de Eventos:

- Origem: MemoryDiagnostics-Results
- ID: 1201
- Resultado: nenhum erro de memória detectado.

## 6. Análise da capacidade de memória

Na aba Desempenho → Memória do Gerenciador de Tarefas, foram identificados:

| Indicador | Resultado |
|---|---:|
| Memória instalada | 8 GB |
| Memória em uso | 7,5 GB |
| Memória disponível | 500 MB |
| Memória confirmada | 10,2 / 13,9 GB |

Os resultados indicaram pressão elevada de memória durante a utilização simultânea dos aplicativos.

## 7. Procedimentos realizados

Com autorização do usuário e por acesso remoto:

- Limpeza de arquivos temporários.
- Remoção de programas desnecessários da inicialização.
- Desativação de recursos extras considerados desnecessários.

Os procedimentos foram realizados sem alteração dos documentos pessoais do usuário.

## 8. Teste após otimização

| Recurso | Antes | Depois |
|---|---:|---:|
| CPU | 35% | 32% |
| Memória RAM | 94% | 88% |
| Disco | 18% | 14% |
| Rede | 3% | 2% |

Foi observada pequena melhora, mas a lentidão ainda persistia durante a utilização simultânea do Excel e navegador.

## 9. Diagnóstico e conclusão

As evidências apontaram possível insuficiência de capacidade de memória RAM para a rotina de trabalho do usuário.

O teste de memória não detectou erros, portanto não houve evidência de defeito físico na RAM durante a verificação.

As otimizações reduziram parcialmente o consumo, mas não solucionaram completamente o problema.

## 10. Encaminhamento

Chamado encaminhado à equipe responsável para avaliar a possibilidade de expansão da memória RAM, considerando compatibilidade do equipamento e necessidades de trabalho.

## 11. Competências praticadas

- Atendimento e comunicação com usuários.
- Investigação de problemas de desempenho.
- Gerenciador de Tarefas.
- Visualizador de Eventos.
- Diagnóstico de memória RAM.
- Acesso remoto autorizado.
- Otimização básica do Windows.
- Documentação e encaminhamento de chamados.

---

**Observação:** Este chamado é uma simulação educacional. Os resultados apresentados representam o cenário fictício utilizado durante o treinamento.
