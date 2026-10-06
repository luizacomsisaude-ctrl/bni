# Painéis de metas da gestão BNI

Painéis das metas da gestão de out/2026 a mar/2027, um por grupo, montados a partir das planilhas de metas.

| Grupo | Painel | Planilha |
|---|---|---|
| BNI Despertar · Gestão 9 | `dashboard/index.html` | `planilhas/METAS_GESTAO_DESPERTAR.xlsx` |
| BNI Excelência · Gestão 23 | `dashboard/excelencia.html` | `planilhas/METAS_GESTAO_EXCELENCIA.xlsx` |
| BNI Euforia · Gestão 6 | `dashboard/euforia.html` | `planilhas/METAS_GESTAO_EUFORIA.xlsx` |
| BNI Eficaz · Gestão 24 | `dashboard/eficaz.html` | `planilhas/METAS_GESTAO_EFICAZ.xlsx` |
| BNI Inovação · Gestão 24 | `dashboard/inovacao.html` | `planilhas/METAS_GESTAO_INOVACAO.xlsx` |

Cada painel mostra as metas planejadas de cada mês e tem campos para lançar o realizado. Os dois usam as mesmas fórmulas; mudam só as premissas de cada grupo (o Excelência também mostra a visão de 85 membros o Euforia, a missão de 40, o Eficaz, a missão de 60, e o Inovação, a missão de 40).

## O que o painel acompanha

Novos membros, total de membros, assiduidade (a partir das faltas do mês), convidados, Um-a-Um, UEG, referências qualificadas, OPNF, renovações e saídas.

As metas planejadas seguem as mesmas fórmulas da planilha:

- Total de membros = mês anterior + novos − saídas previstas − renovações que não devem acontecer (previstas × (1 − taxa de renovação ideal))
- Convidados = total de membros
- Um-a-Um e UEG = membros × reuniões do mês
- Referências qualificadas = membros × reuniões × 1,12
- OPNF = reuniões × membros × valor da cadeira por reunião (OPNF do período anterior ÷ PALMS)
- Faltas máximas = (1 − meta de assiduidade) × membros × reuniões

Qualquer meta planejada pode ser ajustada direto na tabela "Planejado × realizado": clique no valor e digite a nova meta. Ao ajustar o total de membros, as metas que dependem dele e os meses seguintes são recalculados. Apagar o valor volta ao cálculo da planilha.

A seção "Renovantes" guarda os nomes de quem renova a afiliação em cada mês, com a situação de cada um (pendente, renovou, não renovou).

A seção "Valor de cadeira e conversão" mostra a eficiência do time: total de negócios (R$) ÷ ticket médio = quantidade de negócios; quantidade de negócios ÷ referências = taxa de conversão. O total de negócios e as referências são digitados mês a mês num quadro da própria seção (mês sem total digitado usa o OPNF lançado). A meta de conversão usa o OPNF e as referências planejados. Também mostra o valor de cadeira do grupo (OPNF ÷ membros) e o valor da cadeira por reunião.

As premissas (reuniões por mês, novos membros planejados, saídas e renovações previstas, taxas) podem ser editadas no próprio painel, na seção "Premissas das metas".

## Onde os dados ficam salvos

Publicado como Artifact no claude.ai, o painel salva os resultados no banco de dados do próprio artifact, compartilhado com quem tiver acesso de edição. Aberto direto no navegador, a partir deste arquivo, ele salva só no navegador (localStorage).
