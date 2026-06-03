# homer-bart-classification
Classificação de imagens com MLP (PyTorch) — sem CNN

# Classificacao Homer vs Bart — Rede Neural MLP Classificacao binaria de imagens dos
personagens Homer e Bart Simpson utilizando uma rede neural MLP (Multi-Layer
Perceptron) com PyTorch, sem o uso de camadas convolucionais. ## Objetivo Construir e
treinar uma rede neural totalmente conectada capaz de distinguir imagens dos
personagens Homer e Bart Simpson, aplicando tecnicas de regularizacao, data
augmentation e avaliacao de modelos. ## Dataset **Nome:** Neural Networks Homer and
Bart Classification **Fonte:** Kaggle —
juniorbueno/neural-networks-homer-and-bart-classification **Classes:** Homer (0) e
Bart (1) **Formato:** Imagens .bmp organizadas em pastas por classe ## Tecnologias
Utilizadas - Python 3.10+ - PyTorch 2.x + torchvision - scikit-learn (metricas) 
matplotlib + seaborn (visualizacoes) - Pillow (manipulacao de imagens) - Google Colab
(ambiente de execucao) ## Arquitetura do Modelo MLP com 4 camadas densas: Entrada
(12.288) -> fc1 (2.048) -> fc2 (512) -> fc3 (128) -> Saida (2) Regularizacao:
BatchNorm + Dropout progressivo (0.5, 0.4, 0.3) Ativacao: ReLU (camadas ocultas) +
LogSoftmax (saida) ## Resultados | Metrica | Valor | |-------------------|---------| |
Acuracia (Teste) | ~XX% | | F1-Score | ~XX% | | AUC-ROC | ~0.XX | ## Principais
Aprendizados - Overfitting e quase inevitavel com poucos dados — regularizacao e
essencial - Separar os transforms de treino e validacao corretamente impacta a
avaliacao - Checkpoint do melhor modelo e superior a usar o da ultima epoca - Data
Augmentation aumenta a robustez sem custo adicional de coleta ## Como Executar 1.
Clone o repositorio 2. Instale as dependencias: pip install -r requirements.txt 3.
Baixe o dataset do Kaggle (link acima) e extraia em data/ 4. Abra
notebooks/RNA_DL_Classificacao_Homer_vs_Bart.ipynb 5. Execute as celulas em ordem ##
Proximos Passos - Implementar com CNN (ResNet-18) e comparar resultados - Adicionar
interface web com Streamlit ou Gradio - Testar com transfer learning ## Autora
Nathalia Rayanne Lima Araujo Cientista de Dados | Analytics em Auditoria Interna
LinkedIn: linkedin.com/in/nathalia-araujo-78b1b0262
