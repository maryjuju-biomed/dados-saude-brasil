# Dengue em Minas Gerais (2013-2026)

Análise de casos prováveis de dengue notificados em Minas Gerais, com dados públicos do SINAN/DATASUS. Primeiro projeto da minha trilha de aprendizado em análise de dados de saúde.

## Arquivos
- `dengue-sinan-2013-2026.csv` - tabela original exportada do TabNet, sem nenhuma edição (todos os estados, por ano)
- `grafico-dengue-mg.png` - série histórica de Minas Gerais

## O que os dados mostram
- 2024 foi o pior ano da série em MG: 1.658.543 casos prováveis
- 2016 passou de 500 mil casos por apenas 3 mil (503.017)
- Os anos alternam picos e vales - a hipótese de que o El Niño forte tenha contribuído para o pico de 2024 é só uma hipótese; estes dados sozinhos não provam

## Como reproduzir
Consulta feita em 16/11/2026 no TabNet (tabnet.datasus.gov.br), base SINAN - Dengue, com:
- Linha: UF de Notificação
- Coluna: Ano Notificação
- Conteúdo: Casos Prováveis
- Todos os períodos selecionados (2013-2026)

## Limitações (importantes!)
1. 2026 é preliminar: dados até 09/11/2026, sujeitos a revisão (66.659 casos em MG nesta consulta).
2. Casos prováveis = todas as notificações menos os casos descartados. Não equivale a casos confirmados nem a taxa de incidência.
3. Consultas com períodos diferentes podem divergir por causa das semanas epidemiológicas de fronteira (52/53 e 01). Exemplo real deste projeto: a mesma base, na mesma data, retornou 65.674 casos em MG numa consulta "somente 2026" e 66.659 na consulta completa "2013-2026". Este repositório usa o valor da consulta completa, cujo arquivo original está aqui para conferência.

## Fonte
Ministério da Saúde / SVSA - Sistema de Informação de Agravos de Notificação (SINAN), via DATASUS TabNet. Dados disponibilizados em novembro de 2026.

---
Projeto de aprendizado. Feito com apoio de ferramentas de IA para organização e revisão - as perguntas, a leitura dos dados e as conclusões são minhas.
