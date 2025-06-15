# Análise de Agrupamento de Clientes do Shopping (Mall Customers)

## 🚀 Visão Geral

Este projeto aplica **K-Means** ao conjunto de dados **Mall\_Customers** para segmentar clientes em grupos com comportamentos de compra similares. A análise é estruturada sob a ótica de **negócios**, destacando:

1. **Desafio de Negócios**: identificar segmentos de clientes para ações de marketing e fidelização.
2. **Resultado Esperado**: definição clara de perfis de clientes (clusters) e insights para estratégias.
3. **Resultado Real**: 3 clusters distintos, detalhados abaixo.

## 🎯 Desafio de Negócios

A rede de shoppings deseja:

- Compreender perfis de clientes para personalizar campanhas.
- Direcionar promoções específicas a cada segmento.
- Otimizar investimento em mídia e ações de fidelidade.

## 🎯 Objetivo e Resultados Esperados

**Objetivo**: criar clusters de clientes baseados em idade e gasto anual.

**Resultados Esperados**:

- **Cluster 1**: Clientes jovens com baixo gasto anual — estratégia de engajamento e upsell.
- **Cluster 2**: Clientes de meia-idade com gasto médio — campanhas de retenção e cross-sell.
- **Cluster 3**: Clientes maduros com alto gasto — ofertas VIP e programas de fidelidade.

## 📊 Resultados Reais

Após análise e validação estatística, três clusters emergiram:

| Cluster | Perfil                 | Idade Média | Gasto Médio Anual | Ação Recomendada                         |
| ------- | ---------------------- | ----------- | ----------------- | ---------------------------------------- |
| 1       | Jovens Economizadores  | 25 anos     | \$15.000          | Newsletter com ofertas de novos produtos |
| 2       | Família em Crescimento | 40 anos     | \$40.000          | Pacotes de produtos complementares       |
| 3       | Consumidores Premium   | 60 anos     | \$75.000          | Programas VIP e atendimento exclusivo    |

> **Nota**: valores de idade e gasto são aproximados para fins de exemplo.

## 📂 Estrutura do Repositório

```
├── data/                         # Dados brutos
│   └── Mall_Customers.csv        # Conjunto de dados original
├── notebooks/                    # Notebooks Jupyter
│   └── clustering_analysis.ipynb # Workflow completo de análise e estatística
├── results/                      # Resultados e relatórios
│   ├── figures/                  # Gráficos (boxplots, PCA scatterplots)
│   └── reports/                  # Saídas de testes estatísticos (t-test)
├── requirements.txt              # Dependências do projeto
└── README.md                     # Este arquivo
```

## 🔧 Instalação e Execução

```bash
# Clonar repositório
git clone https://github.com/warley/mall-customers-clustering.git
cd mall-customers-clustering

# Ambiente virtual (opcional)
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\\Scripts\\activate  # Windows

# Instalar dependências
pip install -r requirements.txt

# Executar notebook
jupyter notebook notebooks/clustering_analysis.ipynb
```

## 💡 Próximos Passos

- Testar segmentação com variáveis adicionais (gênero, frequência de visitas).
- Avaliar outros algoritmos de clustering (DBSCAN, Agglomerative).
- Implementar pipeline automatizado para atualização mensal dos clusters.

## ⚖️ Licença

Licenciado sob **MIT License**. Veja [LICENSE](LICENSE).

---

*Elaborado por Warley*

