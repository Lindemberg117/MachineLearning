# Preencher Dados Faltantes

Este projeto mostra como carregar um arquivo CSV, identificar valores ausentes (`NaN`) e preenchê-los utilizando a biblioteca **scikit-learn**.

## Passos realizados

1. **Carregar os dados**  
   Utilizamos o **pandas** para ler o arquivo `svbr.csv`, separando as colunas corretamente.

2. **Converter para NumPy**  
   Transformamos o DataFrame em uma matriz NumPy para facilitar a aplicação de técnicas de machine learning.

3. **Tratar valores ausentes**  
   Usamos a classe `SimpleImputer` do **scikit-learn** com a estratégia `"median"`, substituindo valores faltantes pela mediana das colunas numéricas selecionadas.

4. **Atualizar os dados**  
   Os valores ausentes foram preenchidos, mantendo as demais colunas do CSV intactas.

## Bibliotecas utilizadas
- **pandas** → manipulação de dados
- **numpy** → matrizes numéricas
- **scikit-learn** → preenchimento de dados faltantes (`SimpleImputer`)

## Resultado
Ao final, obtemos uma matriz `X` sem valores nulos, pronta para análises ou aplicação de modelos de aprendizado de máquina.
