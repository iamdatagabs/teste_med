# MedVoca — Orientação vocacional médica

Aplicação web estática para apoiar a reflexão sobre interesses, preferências de trabalho e afinidades com especialidades médicas.

## Escopo atual

- Três percursos: Expressa (12 questões), Intermediária (24) e Completa (36).
- Questões de escolha única e múltipla seleção.
- Catálogo com as **55 especialidades médicas reconhecidas pela Comissão Mista de Especialidades (CME)**, conforme a Resolução CFM nº 2.472/2026.
- Pontuação comparativa de afinidade, em escala de 0 a 100, baseada em oito dimensões de atuação.
- Perfil descritivo, dimensões predominantes, leitura comportamental inspirada no DISC e arquétipo narrativo.
- Descrições introdutórias das especialidades e relatório imprimível / exportável como PDF.
- Interface responsiva para desktop e dispositivos móveis.
- Sem backend, cadastro ou transmissão das respostas.

## Como executar

Abra `index.html` em um navegador moderno. Para publicar, habilite GitHub Pages nas configurações do repositório, selecionando a branch principal e a pasta raiz (`/(root)`). O workflow em `.github/workflows/pages.yml` automatiza a publicação em pushes para `main`, desde que GitHub Pages esteja configurado para GitHub Actions.

## Referência regulatória

A lista de especialidades foi conferida com a **Resolução CFM nº 2.472, de 24 de setembro de 2026**, publicada no Diário Oficial da União em 28 de outubro de 2026, que homologa a Portaria CME nº 1/2026 e revoga a Resolução CFM nº 2.380/2024.

- [Resolução CFM nº 2.472/2026 — texto publicado no DOU (PDF)](https://cdn.medblog.estrategiaeducacional.com.br/wp-content/uploads/2026/10/RESOLUCAO-CFM-No-2.472-DE-24-DE-SETEMBRO-DE-2026-RESOLUCAO-CFM-No-2.472-DE-24-DE-SETEMBRO-DE-2026-DOU-Imprensa-Nacional.pdf)
- [Portal CFM — busca de normas](https://portal.cfm.org.br/buscar-normas-cfm-e-crm/)

O catálogo do questionário apresenta as especialidades médicas. **Áreas de atuação são categorias regulatórias distintas** e não são misturadas ao ranking de especialidades.

## Como interpretar a pontuação

As respostas alimentam oito dimensões: diagnóstico, análise, continuidade do cuidado, relação com pessoas, procedimentos, atuação aguda, fisiologia e tecnologia. Cada especialidade possui pesos editoriais nessas dimensões. A pontuação exibida é uma combinação ponderada, normalizada em escala de 0 a 100.

Essa escala serve apenas para ordenar afinidades dentro da ferramenta. Não é percentil, probabilidade, nota de aptidão, previsão de desempenho ou comparação com outros respondentes. Os pesos atuais são hipóteses iniciais e ainda não passaram por validação de conteúdo.

## Limites científicos e éticos

O MedVoca é um **protótipo educativo e exploratório**, não um teste vocacional validado, instrumento psicológico, diagnóstico ou recomendação definitiva de carreira.

- O perfil é uma síntese descritiva das respostas.
- O DISC é apenas uma leitura educativa inspirada nos quatro fatores do modelo; não é uma aplicação oficial ou avaliação psicométrica.
- Os arquétipos são metáforas narrativas, sem pretensão de classificar cientificamente a personalidade.
- As descrições e os pesos das especialidades precisam de revisão por especialistas.
- A pontuação não avalia competência clínica, desempenho acadêmico, saúde mental, aptidão manual ou chance de aprovação em residência.
- A rotina real varia entre serviços, regiões, equipes e subáreas.

## Plano de desenvolvimento e validação

1. **Validade de conteúdo:** painel multidisciplinar de médicos especialistas para revisar cobertura, clareza, pertinência das perguntas e coerência dos pesos.
2. **Entrevistas cognitivas:** estudantes de Medicina respondem e explicam como interpretaram cada item, identificando ambiguidades e alternativas ausentes.
3. **Piloto de usabilidade:** avaliar compreensão, tempo de resposta, acessibilidade, funcionamento móvel e abandono.
4. **Análise exploratória:** examinar distribuição das respostas, itens pouco informativos, consistência e estabilidade teste-reteste quando apropriado.
5. **Revisão do algoritmo:** ajustar pesos com justificativa documentada e comparar resultados com preferências refletidas e experiências de exploração, sem tratar escolha atual como verdade absoluta.
6. **Validação externa:** somente após amostra e desenho adequados, investigar validade, confiabilidade e limites de generalização. Não publicar alegações psicométricas antes dessa etapa.

A participação de estudantes em estudos futuros deverá ocorrer com informação clara, consentimento e avaliação ética institucional quando aplicável.

## Privacidade

As respostas são processadas no navegador e não são transmitidas a uma API. O projeto não solicita nome, e-mail ou outros dados pessoais. O relatório é gerado localmente pelo recurso de impressão do navegador.

## Estrutura

- `index.html`: aplicação, questionário, algoritmo e apresentação dos resultados.
- `README.md`: documentação do projeto.
- `.github/workflows/pages.yml`: publicação automatizada no GitHub Pages.

## Licença e uso

Protótipo em evolução. Antes de uso institucional, pesquisa formal ou divulgação como instrumento de orientação profissional, revisar conteúdo, acessibilidade, referências e requisitos éticos.
