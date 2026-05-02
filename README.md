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
4. **Aplicação e acompanhamento:** Através da plataforma digital da sua corretora/banco ou utilizando o próprio site e aplicativo oficial do Tesouro Direto, você pode realizar as ordens de compra e controlar seus investimentos. É permitido investir até o limite máximo de R$ 2.000.000,00 por mês por pessoa.

Por fim, é preciso se atentar às **tributações e taxas** envolvidas no processo. Os rendimentos do Tesouro Direto estão sujeitos ao Imposto de Renda, que incide através de uma tabela regressiva, cujas alíquotas começam em 22,5% e caem até 15% para investimentos mantidos por mais de 720 dias. Há também a cobrança de IOF, mas apenas se você resgatar o dinheiro nos primeiros 29 dias de aplicação. Além dos impostos, existe uma taxa de custódia cobrada pela B3 pelo serviço de guarda dos títulos, que é provisionada diariamente, embora exista isenção dessa taxa para montantes de até R$ 10.000,00 investidos especificamente no Tesouro Selic.

</details>
<details>
<summary> ❓ <b>Quanto rende o Tesouro Direto comparado à poupança?</b> </summary>

Comparando um cenário de investimento de 5 anos, **o Tesouro Direto apresenta um rendimento expressivamente superior ao da caderneta de poupança**.

Para entender essa diferença na prática, podemos observar uma simulação de cálculo de juros compostos:

- **Poupança:** Considerando uma taxa de 7,97%, o investimento na poupança ao longo de 5 anos gera um rendimento efetivo acumulado de **46,72%** (o equivalente a uma média de 9,34% ao ano).
- **Tesouro Direto (Prefixado):** Utilizando como exemplo um título Tesouro Prefixado (LTN) oferecido no final de abril de 2026 com taxa de 13,88% ao ano e vencimento para 2031. Se você mantiver o título até o vencimento, terá o desconto da menor alíquota de Imposto de Renda, que é de 15%. Deduzindo esse imposto, a sua taxa líquida passa a ser de 11,79% ao ano. Ao final de 5 anos, os juros compostos sobre essa taxa líquida geram um rendimento total de **74,58%** (uma média de 14,91% ao ano).

Neste exemplo, mesmo após descontar o Imposto de Renda, **o título do Tesouro Direto rendeu quase 28 pontos percentuais a mais que a poupança** (74,58% líquido contra 46,72%) no período estipulado.
Cabe lembrar que a Poupança tem sua rentabilidade atrelada à Taxa Referencial (TR) e à Selic, enquanto no Tesouro Direto você pode escolher títulos prefixados, pós-fixados pela Selic ou indexados à inflação (IPCA), o que vai ditar a exata rentabilidade da sua aplicação dependendo do momento da economia e do prazo do investimento.

</details>
<details>
<summary> ❓ <b>Quais os riscos de vender o título antes do vencimento?</b> </summary>

O principal risco de vender um título do Tesouro Direto antes do prazo acordado é o **risco de marcação a mercado**. Isso significa que, ao tentar vender títulos como o Tesouro Prefixado ou o Tesouro IPCA+ de forma antecipada, **o valor que você receberá dependerá do preço do título no mercado no exato momento da venda**, o qual sofre variações de acordo com as expectativas e variáveis econômicas. Se o título estiver desvalorizado em relação ao momento da compra, **essa venda pode resultar em perdas financeiras**.
Além da marcação a mercado, existem outros fatores que você deve considerar ao solicitar o resgate antecipado:

- **Incerteza do preço da venda em horários não úteis:** Se a sua ordem de venda for feita entre 18h e 5h, ou durante finais de semana e feriados, a transação não será fechada na hora. Ela será liquidada com os **preços de abertura do dia útil seguinte**. Nesses períodos fora do horário comercial, as taxas e preços exibidos no site servem apenas como referência e podem sofrer alterações até o momento da liquidação.
- **Suspensão temporária do mercado:** Para proteger o investidor, o Tesouro Direto pode suspender os investimentos e resgates ao longo do dia para garantir que os preços e taxas estejam alinhados com o mercado, o que pode impactar o momento exato em que você consegue realizar a venda.
- **Risco de liquidez:** Embora o Tesouro Direto permita vendas antecipadas, existe sempre o risco de você enfrentar um momento adverso no mercado onde não seja possível executar a sua venda pelo preço oportuno ou mais adequado para sua estratégia.
- **Maior incidência de Impostos e Taxas:** Vender o título mais cedo afeta diretamente o rendimento líquido. Se o resgate ocorrer nos primeiros 29 dias de aplicação, haverá a cobrança de **IOF** sobre os rendimentos. Já o **Imposto de Renda** segue uma tabela regressiva, o que significa que resgates precoces pagam as maiores alíquotas, começando em 22,5% se a venda ocorrer nos primeiros 180 dias. Adicionalmente, a taxa de custódia cobrada pela B3 será imediatamente debitada da sua conta na ocorrência da venda antecipada.

Por todos esses motivos, especialistas recomendam que o investidor se atente bastante ao prazo de vencimento na hora de escolher um título, buscando alinhar a data de resgate aos seus objetivos financeiros.

</details>
<details>
<summary> ❓ <b>Existe valor mínimo para começar a investir?</b> </summary>

Sim, existe um valor mínimo, mas ele não é um valor fixo em reais, pois varia de acordo com o preço do título escolhido no dia da compra.
No Tesouro Direto, o investimento mínimo exigido deve ser múltiplo de **0,01 título**, o que significa que você pode comprar a partir de uma fração de **1% do valor de um título** (já descontando as taxas de serviços cobradas).
Graças a essa regra das frações, o programa se destaca pela sua acessibilidade e democratização, permitindo que os investidores comecem a aplicar o seu dinheiro utilizando quantias bastante baixas. No site oficial, você pode conferir uma tabela com todos os títulos disponíveis, onde é exibido exatamente qual o investimento mínimo em reais para cada opção naquele momento.

</details>
<details>
<summary> ❓ <b>Qual o investimento mínimo em reais para cada título hoje?</b> </summary>

As fontes fornecidas não listam o valor mínimo exato em reais para cada título no dia de hoje.
Como os preços dos títulos sofrem marcação a mercado e oscilam diariamente, o valor mínimo exigido em reais também muda todos os dias. A regra estabelecida pelo programa é que os aportes devem ser múltiplos de 0,01 título, o que corresponde a **1% do valor de um título**.
Para consultar o investimento mínimo exato em reais de cada opção no dia de hoje, você deve acessar o **site oficial do Tesouro Direto**. O portal disponibiliza uma tabela atualizada com todos os títulos disponíveis, onde é possível verificar o preço unitário, as taxas de rentabilidade anual, o prazo de vencimento e o respectivo investimento mínimo exigido em reais. Alternativamente, você também pode checar esses valores na área de investimentos da plataforma digital do seu banco ou corretora.

</details>

### 🩹 "Cicatrizes" e Aprendizados (Troubleshooting)
Durante o desenvolvimento, um ponto de atenção (ou "cicatriz") foi observado no comportamento da ferramenta:

* **Fidelidade aos Dados (RAG):** Achei interessante que, mesmo insistindo na questão do valor mínimo em reais, a ferramenta não inventa nem tenta auferir valores pois não possui essa informação em sua base de fontes. 
* **Comportamento Diferenciado:** Notei um comportamento diferente de outras ferramentas de IA Generativa tradicionais. Acredito que essa precisão e a recusa em "alucinar" dados numéricos voláteis ocorram devido à tecnologia **RAG (Retrieval-Augmented Generation)** usada no NotebookLM, que limita as respostas ao contexto dos documentos fornecidos.

---

## 📖 Miniguia de Estudo (Entrega Final)

Nesta seção, você encontra o resultado final consolidado deste projeto, criado para facilitar o aprendizado e futuras revisões sobre o mercado de renda fixa e o Tesouro Direto. O material foi organizado nos seguintes documentos:

### 📁 Documentos de Estudo (Internos)

*   📝 **[Resumos Estruturados](./resumo.md):** Um compilado direto ao ponto com os principais funcionamentos, vantagens e diferenças entre os títulos do Tesouro Direto.
*   📚 **[Glossário de Conceitos](./glossario.md):** Um dicionário prático para consulta rápida dos principais termos financeiros aprendidos durante o projeto.
*   🤖 **[Prompts Reutilizáveis](./prompts.md):** Um conjunto de prompts pré-configurados para você copiar, colar na IA e realizar novas simulações ou testes de conhecimento.

### 🌐 Materiais de Apoio (Externos)

Para uma visão ainda mais ampla ou para apresentar o projeto a terceiros, consulte os links abaixo:

*   🔗 **[Guia Tesouro Direto](https://notebooklm.google.com/notebook/ca149f9b-500b-406a-b83d-e4bd8fc6f53f/artifact/5f02c897-705c-441a-905e-d59266f2f10c?utm_source=nlm_web_share&utm_medium=google_oo&utm_campaign=art_share_1&utm_content=&utm_smc=nlm_web_share_google_oo_art_share_1_)**
*   🖥️ **[Apresentação Tesouro Direto](https://notebooklm.google.com/notebook/ca149f9b-500b-406a-b83d-e4bd8fc6f53f/artifact/a1951a14-0843-4eb6-aee8-d0cd722f1fbf?utm_source=nlm_web_share&utm_medium=google_oo&utm_campaign=art_share_1&utm_content=&utm_smc=nlm_web_share_google_oo_art_share_1_)**

---

<div align="center">
    Desenvolvido por <strong><a href="https://www.linkedin.com/in/patryck-pereira-5104a6140/">Patryck Pereira</a></strong>.<br>
    Projeto parte do Bootcamp <strong>Riachuelo - Cibersegurança</strong> da plataforma:
    <br><br>
    <a href="https://web.dio.me/home">
        <img src="https://img.shields.io/badge/Desafio-DIO-0077B6?style=for-the-badge" alt="Desafio DIO Badge">
    </a>
</div>
