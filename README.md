# cp1-goodwe-chatbot
Chatbot com IA para gestão de eletropostos em condomínios (EV ChargeOps) – Desafio GoodWe &amp; FIAP 2026.

**Integrantes**

Daniel Vieira Santos - RM: 573326

Gustavo Bitencourt Lopes - RM: 568885

Giovane Salazar Fioravante - RM: 570396

Leonardo Basile Takachi - RM: 569066

# Tecnologias Selecionadas

Linguagem: Python (pela versatilidade e bibliotecas de dados).

IA/LLM: Google Gemini API (devido à integração nativa com o ecossistema Google e alta capacidade de contexto).

Análise de Dados: Pandas (para simular a leitura de logs de consumo dos eletropostos).

Interface: Streamlit ou Flask (para criar uma interface de chat amigável).

# Proposta do Chatbot

O chatbot será focado na solução **EV ChargeOps**, servindo como um assistente operacional para **Síndicos e Gestores Prediais**. 
Ele permitirá:

1. Consultar o status de ocupação das estações de recarga.
2. 
3. Gerar resumos de consumo por unidade/apartamento.
4. 
5. Oferecer suporte técnico básico para erros comuns nos carregadores GoodWe.

# Fluxograma de Funcionamento

*(colocar imagem do fluxograma)*
> [Link para a imagem do Fluxograma]

# Contexto-Base (System Prompt)

"Você é o GoodWe ChargeOps Assistant. Sua função é auxiliar síndicos na gestão de eletropostos residenciais. Use dados fornecidos para calcular faturas e resolver problemas técnicos de primeiro nível. Mantenha um tom profissional e técnico."

# Modelo de Teste (Perguntas Esperadas)

1. "Qual o consumo total do carregador 01 este mês?"
2. 
3. "O apartamento 102 realizou alguma recarga hoje?"
4. 
5. "O que significa a luz vermelha piscando no carregador?"
6. 
7. "Como faço para cadastrar um novo morador no sistema?"
8. 
9. "Gere um relatório de faturamento para o Bloco A."
