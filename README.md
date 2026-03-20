<div align="center">
  <img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/aqua.png" width="100%">
  
  # 🏦 Bank Marketing Classification
  ### Otimização de Campanhas com Random Forest & Optuna
  
  [![Python](https://img.shields.io/badge/Python-3.9+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
  [![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
  [![Optuna](https://img.shields.io/badge/Optuna-4285F4?style=for-the-badge&logo=target&logoColor=white)](https://optuna.org/)

  <p align="center">
    <i>Transformando dados brutos de telemarketing em insights acionáveis e modelos preditivos de alta performance.</i>
  </p>
</div>

---

## 📑 Resumo do Projeto

Este projeto utiliza o dataset **Bank Marketing** (UCI) para prever se um cliente irá aderir a um depósito a prazo. O diferencial aqui é o uso de **Engenharia de Recursos** estratégica e **Otimização Bayesiana** para lidar com o desequilíbrio severo das classes.

### 🏗️ Arquitetura do Modelo
O pipeline foi construído para ser robusto e escalável:

1.  **Pré-processamento:** Limpeza de ruídos e remoção de variáveis com *Data Leakage* (ex: `duration`).
2.  **Tratamento de Dados:** Aplicação de **SMOTE** (Synthetic Minority Over-sampling Technique) para equilibrar a base.
3.  **Tuning:** Otimização de hiperparâmetros via **Optuna** focando na métrica F1-Score.

---

## 📊 Performance Visual

<table align="center">
  <tr>
    <td align="center"><b>Métrica</b></td>
    <td align="center"><b>Resultado</b></td>
    <td align="center"><b>Status</b></td>
  </tr>
  <tr>
    <td>Acurácia Geral</td>
    <td><code>87%</code></td>
    <td>✅</td>
  </tr>
  <tr>
    <td>ROC-AUC</td>
    <td><code>0.784</code></td>
    <td>🚀</td>
  </tr>
  <tr>
    <td>F1-Score (Classe 1)</td>
    <td><code>0.45</code></td>
    <td>📈</td>
  </tr>
</table>

> [!IMPORTANT]
> A remoção da variável `duration` é crucial para evitar o viés de predição, já que a duração da chamada só é conhecida após o desfecho do contato.

---

## 🛠️ Stack Tecnológica

<div style="display: inline-block;">
  <img src="https://img.shields.io/badge/pandas-%23150458.svg?style=flat-square&logo=pandas&logoColor=white">
  <img src="https://img.shields.io/badge/numpy-%23013243.svg?style=flat-square&logo=numpy&logoColor=white">
  <img src="https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=flat-square&logo=Matplotlib&logoColor=black">
  <img src="https://img.shields.io/badge/Seaborn-%23444444.svg?style=flat-square&logo=python&logoColor=white">
</div>

---

## 💻 Como Rodar

```bash
# Clone o repositório
git clone [https://github.com/seu-usuario/seu-repositorio.git](https://github.com/seu-usuario/seu-repositorio.git)

# Instale as dependências
pip install -r requirements.txt

# Execute o Jupyter Notebook
jupyter notebook UCI_market.ipynb
