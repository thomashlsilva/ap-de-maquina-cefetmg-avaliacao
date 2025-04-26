# Otimização de Modelos de ML

## Descrição
Framework para experimentos de aprendizado de máquina com otimização automática de hiperparâmetros (Optuna) e validação cruzada.

## Funcionalidades
- ✅ Cálculo de métricas (F1, Acurácia, Matriz de Confusão).  
- ✅ Suporte a Decision Tree e Random Forest.  
- ✅ Validação cruzada com k-folds.  

## Como Usar
```python
from metodo import ScikitLearnAprendizadoDeMaquina
from avaliacao import Experimento
from sklearn.ensemble import RandomForestClassifier
```

```python
# 1. Carregar dados (ex: df_dados)
# 2. Criar folds
folds = Fold.gerar_k_folds(df_dados, val_k=5, col_classe="target")
# 3. Executar experimento
exp = Experimento(folds, RandomForestClassifier(), OtimizacaoObjetivoRandomForest)
print(f"Macro F1 médio: {exp.macro_f1_avg}")
```
## Instalação de Dependências

Certifique-se de ter o Python e os pacotes necessários instalados:

```bash
apt-get install python3 jupyter python3-pip
pip install -r requirements.txt
```

Atenção: Evite usar sudo com o pip.

### Executando o Jupyter Notebook

```bash
jupyter notebook
```
Abra o notebook fornecido e execute as células conforme as instruções no arquivo.

---

## Créditos

Atividade desenvolvida para a disciplina de Machine Learning do CEFET-MG, Campus Nova Gameleira.

Material baseado nas aulas do professor Daniel Hasan Dalip.