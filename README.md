# 📊 Análise de Métricas de Classificação Binária

Um notebook Python para cálculo e visualização de métricas de modelos de classificação a partir de matrizes de confusão.

## 🚀 Funcionalidades Principais
- **Cálculo Automático**:
  - ✅ Sensibilidade (Recall)
  - ✅ Especificidade
  - ✅ Acurácia
  - ✅ Precisão
  - ✅ F-Score
- **Visualização**:
  - 📈 Matriz de confusão com `sklearn.metrics`
- **Robustez**:
  - 🛡️ Tratamento de divisão por zero
  - 🔢 4 casas decimais de precisão

## 💻 Instalação
1. Clone o repositório:
```bash
git clone https://github.com/danielvlemos/DIO_Desafio_Calculo_de_Metricas_de_Avaliacao_de_Aprendizado_Matriz_de_confusao_plotada.git
```

2. Instale as dependências
 ```bash
   pip install -r requirements.txt
   ```
## 🛠️ Como Usar
```python
from metrics import avaliar_modelo

# Exemplo com valores da matriz de confusão
resultados = avaliar_modelo(VP=50, FN=10, FP=5, VN=35)
print(resultados)
```
## 📊 Saída Esperada
```python
{
    'Sensibilidade (Recall)': 0.8333,
    'Especificidade': 0.8750,
    'Acurácia': 0.8500,
    'Precisão': 0.9091,
    'F-Score': 0.8696
}
```
## 📌 Métricas Calculadas
```bash
Métrica	            Fórmula	               Interpretação
Sensibilidade	      VP / (VP + FN)	       Detecção de casos positivos
Especificidade	      VN / (VN + FP)	       Detecção de casos negativos
Acurácia	      (VP + VN) / Total	       Acertos totais
Precisão	      VP / (VP + FP)	       Confiabilidade dos positivos
F-Score 	      2(PR)/(P+R)	       Balanceamento P/R
```

## 🤝 Como Contribuir
1. Faça um fork do projeto
2. Crie sua branch: git checkout -b minha-feature
3. Commit suas mudanças: git commit -m 'Minha nova feature'
4. Push para a branch: git push origin minha-feature
5. Abra um Pull Request


   
