# Biomechanics-ML
Pipeline de ML com visão computacional para análise de marcha — do vídeo à decisão assistida por IA. Sports2D, scikit-learn e SHAP, enquadrados pelos 8 pilares do framework Reality-Centric AI.

Este repositório abrange inteligência artificial aplicada à biomecânica. O vídeo é processado pelo Sports2D; as variáveis extraídas dos pontos anatômicos alimentam um modelo de machine learning; a ferramenta SHAP explica por que das previsões do modelo. A cada passo, o framework Reality-Centric AI obriga-nos a perguntar quais pressupostos vamos adotar — e quando devemos desconfiar dos dados e do modelo.

## Objetivos de Aprendizagem
Ao final do projeto, seremos capazes de:

1. Executar uma pipeline de pose estimation 2D com Sports2D a partir de um vídeo, extraindo coordenadas articulares e ângulos dos membros superiores e inferiores.
2. **Saber quando confiar nos dados:** Documentar os pressupostos da análise 2D com câmara única, reconhecendo as condições em que os ângulos estimados são suficientemente confiáveis para informar uma decisão clínica e as em que não o são (Pilar 1 — RCAI: modelar o mundo com honestidade sobre suas limitações).
3. **Escolher as variáveis certas, não as mais fáceis:** Construir manualmente features específicas e demonstrar, quantitativamente, que um conjunto pequeno de variáveis clinicamente significativas pode igualar ou superar dezenas de features geradas automaticamente a partir da captura de dados (Pilar 3 — RCAI: adquirir o mínimo de dados necessário, com a qualidade certa).
4. **Avaliar o modelo com o olhar clínico:** treinar e comparar modelos e ir além das métricas padrão: perceber que, num contexto clínico, um falso negativo e um falso positivo não têm o mesmo custo — e que a escolha do modelo deve refletir essa assimetria (Pilar 5 — RCAI: definir o que "bom" significa no contexto real, não no benchmark).
5. **Preparar o modelo para o mundo imperfeito:** Testar a robustez do modelo diante de dados imperfeitos, injetando ruído e avaliando a degradação do desempenho para compreender até que ponto o modelo é robusto às condições reais de captação (Pilar 2 — RCAI: operar com dados reais, não com dados de laboratório).
6. **Explicar para quem precisa de decidir:** Aplicar SHAP para tornar as predições interpretáveis e adaptar essa explicação a diferentes audiências (Pilar 7 — RCAI: a explicação certa para a pessoa certa).
7. **Reconhecer que o modelo não decide sozinho:** Discutir o enquadramento regulatório e ético da utilização de IA baseada em vídeo na tomada de decisão clínica, ou seja, quem é responsável pela decisão final, quais requisitos de validação se aplicam e como garantir que o modelo comunica sua incerteza de forma que o clínico possa agir com segurança (Pilar 6 — RCAI: manter o humano no ciclo, especialmente em domínios de alto risco).
8. Manter o modelo vivo após o deployment — usar o repositório do GitHub para registrar cada versão do pipeline (dados, notebooks, modelos serializados) e detectar quando os dados novos se afastam da distribuição original, sinalizando a necessidade de retreino ou de revisão clínica (Pilar 4 — RCAI: adaptação contínua ao mundo real).
 
## Referências

1. van der Schaar, M. & Rashbass, A. (2023). The case for Reality-centric AI. van der Schaar Lab, University of Cambridge. https://www.vanderschaar-lab.com/the-case-for-reality-centric-ai/
2. Pagnon, D. & Kim, H. (2024). Sports2D: Compute 2D human pose and angles from a video or a webcam. Journal of Open Source Software, 9(101).
3. Lundberg, S. M. & Lee, S.-I. (2017). A unified approach to interpreting model predictions. NeurIPS.
4. Robertson, D. G. E. et al. (2014). Research Methods in Biomechanics (2nd ed.). Human Kinetics.
