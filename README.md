# Biomechanics-ML
Pipeline de ML com visão computacional para análise de marcha. Sports2D, scikit-learn e SHAP, enquadrados pelos pilares do framework [Reality-Centric AI](https://www.vanderschaar-lab.com/the-case-for-reality-centric-ai/) (RCAI).

Abrangeremos IA aplicada à biomecânica. O vídeo é processado pelo [Sports2D](https://github.com/davidpagnon/Sports2D); as variáveis extraídas dos pontos anatômicos alimentam um modelo de machine learning; a ferramenta SHAP nos indica a interpretabilidade do modelo treinado. Por fim, o framework Reality-Centric AI obriga-nos a perguntar quais pressupostos vamos adotar — e quando devemos suspeitar dos dados e do modelo.

<video src="https://raw.githubusercontent.com/mauriciomau0/Biomechanics-ML/refs/heads/main/Content/participante_idoso.mp4" width="720" height="480" controls></video>

**Dados extraídos de um dos participantes do grupo de idosos saudáveis:**

<video src="https://raw.githubusercontent.com/mauriciomau0/Biomechanics-ML/refs/heads/main/Content/participante_idoso.mp4" width="720" height="480" controls></video>

**Dados extraídos de um dos participantes do grupo de amputados:**

## Objetivos de Aprendizagem
Ao final do projeto, seremos capazes de:

## Objetivos de Aprendizagem

- [x] Executar uma pipeline de pose estimation 2D com Sports2D a partir de um vídeo, extraindo coordenadas articulares e ângulos dos membros superiores e inferiores.
- [x] Documentar os pressupostos da análise 2D com câmara única, reconhecendo as condições em que os ângulos estimados são suficientemente confiáveis para informar uma decisão clínica (Pilar 1 — RCAI: modelar o mundo com honestidade sobre suas limitações).
- [x] Reconhecer as condições em que os dados do Sports2D não são suficientes para uma decisão clínica — e saber comunicar essa limitação de forma explícita e rastreável (Pilar 1 — RCAI: modelar o mundo com honestidade sobre suas limitações).
- [x] Construir manualmente features específicas, escolhendo variáveis com significado clínico em vez de estatísticas descritivas geradas automaticamente (Pilar 3 — RCAI: adquirir o mínimo de dados necessário, com a qualidade desejável).
- [x] Treinar modelos de classificação com o scikit-learn, avaliando o desempenho com métricas adequadas ao contexto (Pilar 5 — RCAI: definir o que "bom" significa no contexto real, não no benchmark).
- [x] Aplicar SHAP para tornar as predições do modelo interpretáveis, identificando quais variáveis cinemáticas motivaram cada classificação (Pilar 7 — RCAI: a explicação certa para a pessoa certa).
- [x] Adaptar a explicação do modelo a diferentes audiências — fisioterapeuta, médico e paciente — reconhecendo que interpretar uma predição não é o mesmo que comunicá-la (Pilar 7 — RCAI: a explicação certa para a pessoa certa).
- [x] Identificar quem é responsável pela decisão final e quais requisitos de validação se aplicam (Pilar 6 — RCAI: manter o humano no ciclo, especialmente em domínios de alto risco).
- [x] Garantir que o modelo comunica a sua incerteza de forma que o clínico possa agir com segurança, sem delegar a decisão ao sistema (Pilar 6 — RCAI: manter o humano no ciclo, especialmente em domínios de alto risco).
- [x] Usar o repositório para registar cada versão do pipeline — dados, notebooks e modelos — mantendo rastreabilidade completa após o deployment (Pilar 4 — RCAI: adaptação contínua ao mundo real).
- [ ] Detectar quando os dados novos se afastam da distribuição original, sinalizando a necessidade de retreino ou de revisão clínica (Pilar 4 — RCAI: adaptação contínua ao mundo real).
 
## Referências

1. van der Schaar, M. & Rashbass, A. (2023). The case for Reality-centric AI. van der Schaar Lab, University of Cambridge. https://www.vanderschaar-lab.com/the-case-for-reality-centric-ai/
2. Pagnon, D. & Kim, H. (2024). Sports2D: Compute 2D human pose and angles from a video or a webcam. Journal of Open Source Software, 9(101).
3. Lundberg, S. M. & Lee, S.-I. (2017). A unified approach to interpreting model predictions. NeurIPS.
4. Robertson, D. G. E. et al. (2014). Research Methods in Biomechanics (2nd ed.). Human Kinetics.
