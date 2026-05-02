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
   
O **Tesouro Direto** é um programa criado em 2002 pela Secretaria do Tesouro Nacional em parceria com a B3 (antiga CBLC) que permite a pessoas físicas investirem em títulos da dívida pública federal. Na prática, **ao investir no Tesouro Direto, você está emprestando dinheiro para o governo federal** e, em troca, recebe esse valor de volta acrescido de juros que variam conforme o tipo de título e o prazo.
Trata-se de uma modalidade de **renda fixa muito segura**, pois conta com a garantia do próprio Tesouro Nacional, apresentando o menor risco de crédito do mercado, conhecido como risco soberano. Além da alta segurança, o Tesouro Direto destaca-se pela **alta liquidez e pela acessibilidade**, democratizando o investimento ao permitir que você inicie com quantias baixas, já que é possível comprar frações a partir de 1% do valor de um título.

Para decidir onde aplicar, é importante conhecer os **tipos de títulos disponíveis**:

- **Tesouro Selic**: Título pós-fixado em que a rentabilidade acompanha a taxa básica de juros da economia. Por ter baixa volatilidade e altíssima liquidez, é considerado o título ideal para a formação de reserva de emergência.
- **Tesouro Prefixado**: Possui uma taxa de juros fixa e determinada no momento da compra. É ideal para investidores que desejam ter a previsibilidade de saber exatamente quanto irão receber na data de vencimento do título.
- **Tesouro IPCA+**: Oferece proteção contra a inflação, garantindo o poder de compra, pois seu rendimento é composto pela variação da inflação (IPCA) somada a uma taxa de juros fixa. É altamente indicado para a formação de reservas financeiras de longo prazo e planejamento de compras futuras.
- **Tesouro RendA+ e Tesouro Educa+**: O RendA+ foi criado especificamente para o planejamento de aposentadoria, oferecendo pagamentos periódicos a partir de uma determinada data, enquanto o Educa+ é voltado para acumular e financiar com segurança os recursos para a educação.

**Como investir no Tesouro Direto em 4 passos**:

1. **Simulação:** Acesse o site oficial do Tesouro Direto e utilize a função Simulador, que ajuda a recomendar um título de acordo com os seus prazos e objetivos financeiros.
2. **Cadastro em uma instituição:** Para investir, você precisa ser residente no Brasil e possuir conta em uma instituição financeira. Cadastre-se em um banco ou corretora de valores que seja habilitada para negociar os títulos. Vale notar que diversas corretoras e bancos isentam os investidores de taxas de administração.
3. **Transferência de recursos:** Transfira o valor que você deseja investir para a conta desse banco ou corretora.
4. Aplicação e acompanhamento:** Através da plataforma digital da sua corretora/banco ou utilizando o próprio site e aplicativo oficial do Tesouro Direto, você pode realizar as ordens de compra e controlar seus investimentos. É permitido investir até o limite máximo de R$ 2.000.000,00 por mês por pessoa.

Por fim, é preciso se atentar às **tributações e taxas** envolvidas no processo. Os rendimentos do Tesouro Direto estão sujeitos ao Imposto de Renda, que incide através de uma tabela regressiva, cujas alíquotas começam em 22,5% e caem até 15% para investimentos mantidos por mais de 720 dias. Há também a cobrança de IOF, mas apenas se você resgatar o dinheiro nos primeiros 29 dias de aplicação. Além dos impostos, existe uma taxa de custódia cobrada pela B3 pelo serviço de guarda dos títulos, que é provisionada diariamente, embora exista isenção dessa taxa para montantes de até R$ 10.000,00 investidos especificamente no Tesouro Selic.

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
