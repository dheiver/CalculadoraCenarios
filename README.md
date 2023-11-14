# Calculadora de Cenários Financeiros

Este é um projeto que inclui uma classe `CalculadoraCenarios` em Python para calcular e analisar diferentes cenários financeiros com base em parâmetros fornecidos. A classe permite que você simule diferentes situações financeiras ao longo de um período de cinco anos e gere resultados em forma de um DataFrame do Pandas.

## Como Usar

Siga as etapas abaixo para usar a classe `CalculadoraCenarios` em seu projeto:

1. Importe a biblioteca Pandas e a classe `CalculadoraCenarios` em seu código:

```python
import pandas as pd

class CalculadoraCenarios:
    # ... (código da classe)
```

2. Crie instâncias da classe `CalculadoraCenarios` com os parâmetros desejados para seus cenários financeiros:

```python
# Exemplo de criação de cenários
cenario_lucro1 = CalculadoraCenarios(750000, 1062500, 416250, 0.5, 0.2)
cenario_lucro2 = CalculadoraCenarios(900000, 1062500, 416250, 0.5, 0.2)
cenario_prejuizo1 = CalculadoraCenarios(375000, 1062500, 416250, 0.5, 0.2)
cenario_prejuizo2 = CalculadoraCenarios(500000, 1062500, 416250, 0.5, 0.2)
```

3. Chame o método `calcular_cenario()` para calcular os resultados financeiros de cada cenário:

```python
# Exemplo de cálculo de cenários
df_lucro1 = cenario_lucro1.calcular_cenario()
df_lucro2 = cenario_lucro2.calcular_cenario()
df_prejuizo1 = cenario_prejuizo1.calcular_cenario()
df_prejuizo2 = cenario_prejuizo2.calcular_cenario()
```

4. Exiba os resultados dos cenários financeiros:

```python
# Exemplo de exibição dos resultados
print("Cenário Lucro 1:")
print(df_lucro1)
print("\n")

# Repita o processo para os outros cenários
```

## Parâmetros da Classe `CalculadoraCenarios`

A classe `CalculadoraCenarios` aceita os seguintes parâmetros no momento da criação de uma instância:

- `receitas_iniciais`: Receitas iniciais do cenário.
- `custos_operacionais_iniciais`: Custos operacionais iniciais do cenário.
- `depreciacao_amortizacao_inicial`: Depreciação e amortização inicial do cenário.
- `taxa_crescimento_receitas`: Taxa de crescimento anual das receitas.
- `taxa_reducao_custos`: Taxa de redução anual dos custos.

## Exemplo de Saída

Os resultados financeiros são apresentados em forma de um DataFrame do Pandas com informações para cada ano dos cenários, incluindo receitas, custos operacionais, depreciação, lucro bruto, lucro operacional, imposto de renda e lucro líquido.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para obter detalhes.

## Contribuições

Contribuições são bem-vindas. Sinta-se à vontade para criar problemas (issues) ou solicitações de pull (pull requests) para melhorar o projeto.
