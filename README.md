# DIO-Desafio-NotebookLM
# 💰 Guia básico de investimento no Tesouro Direto

![Status do Projeto](https://img.shields.io/badge/Status-Completo-brightgreen)
![Categoria](https://img.shields.io/badge/Categoria-Educação%20Financeira-blue)
![Risco](https://img.shields.io/badge/Risco-Soberano-gold)

---

## 📌 Contexto

O **Tesouro Direto** é um programa da Secretaria do Tesouro Nacional criado em 2002 em parceria com a B3. 
Na prática, trata-se de uma modalidade de renda fixa onde você empresta dinheiro ao governo federal em troca de uma taxa de juros.

**Principais pilares:**
- **Segurança:** Garantia do Tesouro Nacional (Risco Soberano).
- **Acessibilidade:** Investimentos a partir de valores baixos.
- **Liquidez:** Possibilidade de venda dos títulos de volta ao governo.

---

## 🎯 Objetivos de Estudo

O conteúdo deste guia foi desenhado para que o leitor consiga:

1.  **Entender o Fluxo:** Desde o cadastro em corretoras/bancos até a liquidação da compra.
2.  **Analisar Vantagens:** Focar em segurança, liquidez secundária e acessibilidade.
3.  **Gerenciar Riscos:** Identificar o impacto da **Marcação a Mercado**, incidência de IR e taxas de custódia da B3.
4.  **Diferenciar Ativos:**
    * **Tesouro Selic:** Pós-fixado ideal para reserva de emergência.
    * **Tesouro IPCA+:** Proteção real contra a inflação.
    * **Tesouro Prefixado:** Taxa fixa conhecida no momento da compra.
5.  **Simular Rentabilidade:** Comparar ganhos reais contra a Poupança utilizando cálculos de juros compostos.

---

## 📚 Fontes

O material base para criação do notebook foi extraído das seguintes referências:

| Fonte | Origem | Descrição |
| :--- | :--- | :--- |
| **Vantagens e Desvantagens** | [Bora Investir (B3)] | Detalhes sobre benefícios, riscos e passo a passo prático. |
| **Como Investir** | [ANBIMA] | Guia estrutural sobre remuneração, custos e tributação (IR/IOF). |
| **Diretrizes Institucionais** | [CAIXA] | Informações sobre horários de liquidação e isenções de custódia. |
| **Análise Financeira** | [Arquivo Interno](./calculo-juros-compostos.md) | Cálculos matemáticos comparando os rendimentos da Poupança e do Tesouro Direto Pré-fixado. |

---

# 🛠️ Engenharia de Prompts e "Cicatrizes"

Nesta seção, documento o raciocínio por trás da construção das informações e como a Inteligência Artificial foi guiada para gerar o conteúdo deste guia.

### 🧠 Estratégia de Interação
Como o objetivo deste projeto é ser um guia básico para iniciantes, optei por utilizar **perguntas simples e diretas** ao invés de prompts super estruturados. A intenção foi simular as dúvidas reais de um usuário comum que está começando a explorar o Tesouro Direto.

As perguntas feitas ao **NotebookLM** foram:
<details>
<summary> ❓ <b>O que é o Tesouro Direto e como investir?</b> </summary>
</details>
<details>
<summary> ❓ <b>Quanto rende o Tesouro Direto comparado à poupança?</b> </summary>
</details>
<details>
<summary> ❓ <b>Quais os riscos de vender o título antes do vencimento?</b> </summary>
</details>
<details>
<summary> ❓ <b>Existe valor mínimo para começar a investir?</b> </summary>
</details>
<details>
<summary> ❓ <b>Qual o investimento mínimo em reais para cada título hoje?</b> </summary>
</details>

### 🩹 "Cicatrizes" e Aprendizados (Troubleshooting)
Durante o desenvolvimento, um ponto de atenção (ou "cicatriz") foi observado no comportamento da ferramenta:

* **Fidelidade aos Dados (RAG):** Achei interessante que, mesmo insistindo na questão do valor mínimo em reais, a ferramenta não inventa nem tenta auferir valores pois não possui essa informação em sua base de fontes. 
* **Comportamento Diferenciado:** Notei um comportamento diferente de outras ferramentas de IA Generativa tradicionais. Acredito que essa precisão e a recusa em "alucinar" dados numéricos voláteis ocorram devido à tecnologia **RAG (Retrieval-Augmented Generation)** usada no NotebookLM, que limita as respostas ao contexto dos documentos fornecidos.
