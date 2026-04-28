# CP2hercules# Projeto: Personal Trainer Virtual - Consultoria Inteligente 🏋️‍♂️

## 1. Nome do Projeto e Domínio
**Nome do Projeto:** FitBot AI – Seu Personal Trainer 24h.
**Domínio:** Saúde, Bem-estar e Tecnologia. O projeto foca na aplicação de Inteligência Artificial Generativa para democratizar o acesso a orientações de exercícios físicos e rotinas de treino personalizadas via chatbot.

## 2. Integrantes
* **Kevin Rodrigues de melo** — RM: 571777
* **Luan de Araujo Carneiro** — RM: 573691
* **Raul sampaio Mochnacs Arruda** — RM: 573523
* **Pedro sampaio Mochnacs Arruda** — RM: 573522
* **Lucas Garcia de Britto** — RM: 571768

## 3. Justificativa
A escolha deste domínio fundamenta-se na crescente busca por autonomia no cuidado com a saúde e na dificuldade que muitos iniciantes enfrentam ao frequentar ambientes de academia sem suporte contínuo. 

Desenvolvemos este chatbot para atuar como um assistente de primeira linha, capaz de ajustar sugestões de exercícios com base no nível de experiência e limitações do usuário. O objetivo é utilizar o processamento de linguagem natural para transformar diretrizes técnicas de educação física em diálogos acessíveis, motivadores e seguros, preenchendo a lacuna entre o desejo de treinar e a falta de informação prática imediata.

---

## 4. Dataset
 O data set foi construído com base em 12 exemplos de perguntas e respostas para treinar o chatbot para responder perguntas sobre musculação, os dados foram rotulados e categorizados em 5 domínios principais: Suporte Técnico, Metodologia, Treino de Inferiores, Treino de Superiores e Progressão de Carga.


* **Construção:** Os dados foram organizados em uma lista de dicionários com pares de `pergunta` e `resposta`.
* **Categorias incluídas:**
 Dúvidas e Suporte Técnico: 4 exemplos
Conceitos e Metodologia: 2 exemplos
Fichas de Treino (Inferiores): 4 exemplos
Fichas e Dúvidas (Superiores): 6 exemplos
Progressão em Multiarticulados: 5 exemplos

* **Quantidade:** O modelo utiliza **21 exemplos de alta qualidade** para manter a precisão das orientações.

## 5. System Prompt
O **System Prompt** atua como a diretriz mestra de comportamento do assistente, configurado no `Modelfile` do Ollama.

* **Decisões de Design:**
    * **Identidade:** O bot foi instruído a ser um assistente amigável, empático e objetivo.
    * **Linguagem:** Uso obrigatório de português brasileiro e emojis relevantes para humanizar o atendimento.
    * **Segurança:** Regras estritas para nunca prometer resultados impossíveis e sempre orientar o suporte humano em caso de dúvidas críticas.
* **Parâmetros de Geração:**
    * `temperature 0.7`: Ajustada para permitir respostas naturais sem perder o rigor técnico.
    * `num_predict 300`: Definido para manter as respostas diretas e evitar fugas do tema.

## 6. Comparação Base vs. Customizado
6. Comparação Base vs. Customizado
Abaixo, detalhamos as diferenças de comportamento entre o modelo genérico (Llama 3.2:1b) e a versão personalizada (FitBot), demonstrando a eficácia da engenharia de prompt aplicada.

Exemplo 1: Segurança e Lesão
Pergunta do Usuário: "Senti uma dor estranha no ombro durante o supino."

Resposta Modelo Base: "A dor no ombro durante exercícios de peito pode ser causada por má postura ou excesso de peso. Tente reduzir a carga ou procure um profissional se a dor não passar."

Resposta Modelo Customizado (FitBot): "Atenção aqui! ⚠️ Pare o exercício imediatamente. Verifique se seus ombros estão encaixados (retratados) no banco. Se a dor persistir, descanse a articulação hoje. Segurança em primeiro lugar! 🛡️"

Diferencial: O FitBot prioriza a interrupção imediata (segurança) e dá uma instrução técnica específica (retratação escapular).


## 7. Aprendizados
* **Integrante 1:*Kevin Rodrigues de melo* (Fiquei responsável pela estruturação da documentação e interface do projeto. Aprendi que a clareza em um arquivo README é vital para a reprodutibilidade do software, utilizando a linguagem Markdown para organizar hierarquicamente as informações técnicas, justificativas e guias de preenchimento. Compreendi como traduzir processos complexos (como a configuração de modelos de IA) em uma comunicação acessível para usuários e outros desenvolvedores que visualizarem o repositório no GitHub.).
  
* **Integrante 2:Pedro Sampaio Mochnacs Arruda Aprendi como um chatbot pode ser treinado através de exemplos e como o chatbot aprende e entende padrões
  
* **Integrante 3:** (Escreva aqui um parágrafo sobre o que você aprendeu tecnicamente ou em grupo durante o desenvolvimento).
