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
O dataset foi desenvolvido em Python e integrado ao modelo através de uma estrutura de mensagens (*few-shot*), garantindo que o bot aprenda com exemplos práticos antes de interagir com o usuário.

* **Construção:** Os dados foram organizados em uma lista de dicionários com pares de `pergunta` e `resposta`.
* **Categorias incluídas:**
    * Dúvidas e Suporte Técnico (Ex: conexão mente-músculo e dores no treino).
    * Conceitos e Metodologia (Ex: divisões de treino para iniciantes).
    * Fichas de Treino (Ex: rotinas de membros inferiores e superiores).
    * Progressão de Carga (Ex: técnicas para evoluir na barra fixa).
* **Quantidade:** O modelo utiliza **12 exemplos de alta qualidade** para manter a precisão das orientações.

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
*(Utilize este espaço para colocar uma tabela ou imagens comparando a resposta da IA padrão com a resposta da sua IA personalizada.)*

| Pergunta do Usuário | Resposta Modelo Base | Resposta Modelo Customizado |
| :--- | :--- | :--- |
| Exemplo de pergunta | Resposta padrão... | Resposta com sua personalidade... |

## 7. Aprendizados
* **Integrante 1:*Kevin Rodrigues de melo* (Fiquei responsável pela estruturação da documentação e interface do projeto. Aprendi que a clareza em um arquivo README é vital para a reprodutibilidade do software, utilizando a linguagem Markdown para organizar hierarquicamente as informações técnicas, justificativas e guias de preenchimento. Compreendi como traduzir processos complexos (como a configuração de modelos de IA) em uma comunicação acessível para usuários e outros desenvolvedores que visualizarem o repositório no GitHub.).
* **Integrante 2:** (Escreva aqui um parágrafo sobre o que você aprendeu tecnicamente ou em grupo durante o desenvolvimento).
* **Integrante 3:** (Escreva aqui um parágrafo sobre o que você aprendeu tecnicamente ou em grupo durante o desenvolvimento).
