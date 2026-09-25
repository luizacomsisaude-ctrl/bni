# BNI Despertar · Gestão 9

Painel de metas da Gestão 9 do BNI Despertar, de out/2026 a mar/2027, montado a partir da planilha `planilhas/METAS_GESTAO.xlsx`.

- `dashboard/index.html`: o painel. Mostra as metas planejadas de cada mês e tem campos para lançar o realizado.
- `planilhas/METAS_GESTAO.xlsx`: a planilha de metas original.

## O que o painel acompanha

Novos membros, total de membros, assiduidade (a partir das faltas do mês), convidados, Um-a-Um, UEG, referências qualificadas, OPNF, renovações e saídas.

As metas planejadas seguem as mesmas fórmulas da planilha:

- Total de membros = mês anterior + novos − saídas previstas − renovações que não devem acontecer (previstas × (1 − 45%))
- Convidados = total de membros
- Um-a-Um e UEG = membros × reuniões do mês
- Referências qualificadas = membros × reuniões × 1,12
- OPNF = reuniões × membros × valor da cadeira por reunião (OPNF do período anterior ÷ PALMS)
- Faltas máximas = (1 − 95%) × membros × reuniões

As premissas (reuniões por mês, novos membros planejados, saídas e renovações previstas, taxas) podem ser editadas no próprio painel, na seção "Premissas das metas".

## Onde os dados ficam salvos

Publicado como Artifact no claude.ai, o painel salva os resultados no banco de dados do próprio artifact, compartilhado com quem tiver acesso de edição. Aberto direto no navegador, a partir deste arquivo, ele salva só no navegador (localStorage).
