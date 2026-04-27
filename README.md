#  cp1-goodwe-chatbot
Chatbot com IA para gestão de eletropostos em condomínios (EV ChargeOps) – Desafio GoodWe & FIAP 2026.

##  Integrantes
* **Daniel Vieira Santos** - RM: 573326
* **Gustavo Bitencourt Lopes** - RM: 568885
* **Giovane Salazar Fioravante** - RM: 570396
* **Leonardo Basile Takachi** - RM: 569066

##  Tecnologias Selecionadas
* **Linguagem:** Python
  * *Justificativa:* Utilizado pela versatilidade e robustez no tratamento de dados e integração de APIs.
* **IA/LLM:** Google Gemini API
  * *Justificativa:* Escolhido pela alta capacidade de processamento de contexto e integração nativa com ferramentas de análise.
* **Análise de Dados:** Pandas
  * *Justificativa:* Biblioteca essencial para simular a leitura de bancos de dados de consumo e gerar relatórios precisos para o síndico.
* **Interface:** Streamlit ou Flask
  * *Justificativa:* Para garantir uma interface de usuário (UI) simples, funcional e de rápido desenvolvimento.

##  Proposta do Chatbot
O chatbot será focado na solução **EV ChargeOps**, servindo como um assistente operacional para **Síndicos e Gestores Prediais**.
Ele permitirá:
1. Consultar o status de ocupação e disponibilidade das estações em tempo real.
2. Gerar resumos detalhados de consumo por unidade/apartamento para rateio de custos.
3. Oferecer suporte técnico de primeiro nível para erros comuns e manutenção preventiva nos carregadores GoodWe.

##  Fluxograma de Funcionamento
O fluxo operacional compreende a entrada da dúvida do gestor, a filtragem de dados via Pandas, o processamento lógico pelo Gemini e a entrega da solução contextualizada.

<img width="615" height="421" alt="fluxograma" src="https://github.com/user-attachments/assets/0d893fcb-db5b-43e6-858e-846011fc84da" />

##  Contexto-Base (System Prompt)
"Você é o GoodWe ChargeOps Assistant, um especialista técnico em gestão de eletropostos residenciais. Sua missão é auxiliar síndicos na operação do sistema EV ChargeOps. Use os dados de logs fornecidos para cálculos de faturamento e siga os manuais da GoodWe para suporte técnico. Mantenha um tom profissional, direto e prestativo."

##  Modelo de Teste (Perguntas e Respostas Esperadas)
1. **Pergunta:** "Qual o consumo total do carregador 01 este mês?"
   * **Resposta esperada:** O bot deve realizar a soma dos kWh registrados na estação 01 no período atual e retornar o valor total.
2. **Pergunta:** "O apartamento 102 realizou alguma recarga hoje?"
   * **Resposta esperada:** O bot deve consultar o log de presença diário e informar o horário da última sessão do morador.
3. **Pergunta:** "O que significa a luz vermelha piscando no carregador?"
   * **Resposta esperada:** O bot deve identificar o código de erro e sugerir o reset do sistema ou a verificação do aterramento.
4. **Pergunta:** "Como faço para cadastrar um novo morador no sistema?"
   * **Resposta esperada:** O bot deve fornecer o passo a passo técnico para inclusão de novas tags de acesso ou usuários no app.
5. **Pergunta:** "Gere um relatório de faturamento para o Bloco A."
   * **Resposta esperada:** O bot deve agrupar o consumo de todas as unidades do Bloco A e apresentar o custo total baseado na tarifa de energia local.
