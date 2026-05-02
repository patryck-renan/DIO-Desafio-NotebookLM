# Análise Financeira: Poupança vs. Tesouro Direto Pré-fixado

> **Documento criado por:** Patryck Pereira
> **Descrição:** Cálculos de matemática financeira para comparação de Poupança X Tesouro Direto Pré-fixado.

## 1. Análise de Rendimento da Poupança

O rendimento atual da poupança é de 0.5% ao mês + TR (Taxa Referencial). A TR varia a cada ano, esteve zerada entre 2018 e 2020, e o total acumulado no ano de 2025 foi de 1.97% (fonte: [Brasil Indicadores](https://brasilindicadores.com.br/tr)).

Utilizando o valor da TR de 2025 temos uma taxa de juros anual de 7,97%. Para entendermos melhor o poder dos juros compostos vamos fazer um cálculo para descobrir o percentual de rendimento da poupança ao longo de cinco anos.

### 1.1 Cálculo dos Juros Compostos (Poupança)

Para o cálculo de juros compostos (juros sobre juros) fazemos a divisão da taxa de juros por 100, no caso 7,97 dividido por 100:

$$\frac{7,97}{100} = 0,0797$$

Somamos esse resultado a 1, que representa o principal, ou seja, o valor investido, e então elevamos o resultado dessa soma ao período, no nosso caso 5 anos.

$$(1 + 0,0797)^5 = 1,0797^5 = 1,4672$$

Agora diminuímos 1 desse resultado e multiplicamos por 100.

$$(1,4672 - 1) \times 100 = 46,72\%$$

**Conclusão da Poupança:** Ou seja, o rendimento efetivo nesse investimento seria 46,72% em 5 anos, ou 9,34% ao ano.

---

## 2. Análise de Rendimento do Tesouro Direto Pré-fixado (LTN)

Para compararmos com o título do tesouro pré-fixado LTN utilizamos os dados disponíveis no [histórico oficial do Tesouro Direto](https://www.tesourodireto.com.br/produtos/dados-sobre-titulos/historico-de-precos-e-taxas).

No dia 30/04/2026 a taxa de juros para investimento nesse título era de 13,88% ao ano, com vencimento em 2031, ou seja, comprando esse título garantimos esse rendimento anual até 2031. Levando em conta que você permaneça com o título até o vencimento, a taxa de imposto de renda será de 15% sobre os rendimentos.

### 2.1 Cálculo da Taxa Líquida (Tesouro Direto)

Nesse caso para calcular a taxa líquida utilizamos o seguinte cálculo.

$$\text{Taxa de juros} \times \frac{100 - \text{Taxa de IR (15)}}{100}$$

Aplicando os valores:

$$13,88 \times 0,85 = 11,79\%$$

### 2.2 Cálculo dos Juros Compostos (Tesouro Direto)

Fazendo o mesmo cálculo que fizemos com a Poupança temos o seguinte:

$$1,1179^5 = 1,7458$$

**Conclusão do Tesouro Direto:** Ou seja 74,58% ao ano = 14,91% a.a.