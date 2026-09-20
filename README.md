# Eleicoes2026

Este repositório reúne prompts prontos para uso em LLMs (como ChatGPT, Claude, Gemini, DeepSeek, etc.) voltados à **pesquisa e análise técnica de candidatos às Eleições 2026 no Brasil**. Cada arquivo orienta a inteligência artificial a agir como cientista político e pesquisador, com critérios objetivos de filtragem — registro no TSE, viabilidade fiscal, histórico de gestão, compromisso democrático e ficha limpa — e a gerar um relatório comparativo dos melhores candidatos para a sua região.

O objetivo é compartilhar estes arquivos para que **qualquer pessoa** possa copiar o prompt para a LLM de sua preferência e avaliar, de forma crítica e fundamentada, os candidatos do seu estado e da sua região. Os prompts produzem uma **análise técnica**, não uma recomendação de voto.

> **Estes prompts NÃO são propaganda eleitoral.** Não realizam recomendação de voto e não são vinculados a partidos, campanhas ou candidatos. São uma ferramenta de **análise técnica**, livre e educativa, cujo resultado é **gerado por IA** e deve ser verificado nas fontes oficiais.

> **Aviso importante:** Os relatórios são gerados **sinteticamente por IA** (conteúdo não humano) e não constituem propaganda, endosso, recomendação de voto ou informação oficial do processo eleitoral. Consulte sempre as fontes oficiais listadas em [Fontes oficiais](#fontes-oficiais) e o portal do TSE antes de qualquer decisão.

## Prompts disponíveis

| Arquivo | Cargo | Escopo da análise | Primeira pergunta feita pela LLM |
|---|---|---|---|
| [`./presidente.md`](./presidente.md) | Presidente da República | Nacional, com opção de recorte por região/estado e áreas temáticas | "Você deseja uma análise geral em nível nacional, ou quer focar nos impactos das propostas dos candidatos à Presidência para alguma região/estado específico e em áreas temáticas prioritárias?" |
| [`./governadores.md`](./governadores.md) | Governador de Estado | Estadual (UF), com possibilidade de indicar região/município de interesse | "Qual é o Estado (UF) [e, se desejar, qual região ou município de interesse prioritário] cujos candidatos a Governador em 2026 você deseja analisar?" |
| [`./senadores.md`](./senadores.md) | Senador Federal | Estadual (UF) | "Qual é o Estado (UF) [e, se houver, a região/cidade prioritária] cujos candidatos ao Senado em 2026 você deseja analisar?" |
| [`./deputados.md`](./deputados.md) | Deputado Estadual e Deputado Federal | Regional (região e até 2 cidades) | "Qual é a região e quais são as cidades (máximo 2) que você deseja analisar?" |

Cada prompt segue a mesma estrutura: define o papel da LLM, aplica a "Regra número 1" (não gerar o relatório antes de ouvir a sua resposta), filtra rigorosamente as candidaturas por critérios técnicos e democráticos e entrega um relatório com painel, tabela de avaliação de 0 a 10, gráficos ASCII, quadro de exclusões e lacunas de acompanhamento.

## Como usar

1. Abra o arquivo do cargo que você quer analisar (ex.: [`./governadores.md`](./governadores.md)).
2. Copie todo o conteúdo do arquivo (Ctrl+A / Ctrl+C) e cole em qualquer LLM de sua preferência.
3. A LLM fará uma primeira pergunta de direcionamento (região, estado e/ou cidades). Responda com o seu caso.
4. Aguarde o relatório técnico e revise os dados nas fontes oficiais indicadas em [Fontes oficiais](#fontes-oficiais).

> **Sobre recusas de resposta:** algumas LLMs podem se recusar a gerar a tabela comparativa por tratar a análise como recomendação de voto. Os prompts já incluem uma "Regra número 3" que declara explicitamente que o relatório é **análise técnica, não recomendação de voto** — se a sua LLM recusar, releia essa regra no arquivo e reenvie o prompt; o pedido é descritivo e não exige recomendação de voto.

## Conformidade e transparência

- **Dados oficiais:** a análise de registro e a filtragem utilizam exclusivamente dados oficiais (TSE / DivulgaCandContas).
- **Conteúdo sintético:** todo relatório é gerado sinteticamente por IA e rotulado como análise automática — não é conteúdo humano nem declaração oficial.
- **Sem desinformação:** lacunas de dados devem ser informadas, nunca preenchidas por suposição.
- **Verificação:** confira sempre os resultados no portal oficial do TSE e nas fontes indicadas abaixo.

## Fontes oficiais

Os prompts referenciam e orientam a verificação nas seguintes fontes oficiais:

- **TSE / DivulgaCandContas** — registro das candidaturas, situação no processo eleitoral, planos de governo e prestação de contas.
- **Tesouro Nacional (Siconfi/STN)** — situação fiscal dos estados e capacidade de endividamento (Capag).
- **TCU / TCE** — julgamento de contas de gestão dos candidatos.
- **IFI / Senado** — auditorias e análises fiscais independentes.
- **Portais da transparência** — verificação de emendas, execução de verbas e votações.

> **Lembre-se:** a análise gerada pela LLM é um ponto de partida. Valide as informações nas fontes oficiais — a decisão de voto é sempre sua.

## Licença

Distribuído sob a licença [MIT](./LICENSE). Consulte o arquivo [LICENSE](./LICENSE) para os termos completos.