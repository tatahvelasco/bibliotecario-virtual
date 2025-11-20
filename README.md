# 📚 Agente Bibliotecário Virtual 📚

## 📝 Descrição
O **Bibliotecário Virtual** é um agente digital desenvolvido no **Azure AI Foundry** para recomendar livros com base no gênero literário solicitado pelo usuário.  
Ele utiliza uma **base de dados curada com 200 obra** de diferentes estilos, épocas e autores. Cada recomendação inclui:

- **Título e autor**  
- **Sinopse original da base** (sem reescrever ou resumir)  
- **Complexidade da leitura** (Iniciante, Intermediário, Avançado)  
- **Motivo para ler** (curadoria que explica o valor da obra)

Esse projeto foi pensado para apoiar estudantes, vestibulandos e leitores curiosos, oferecendo não apenas indicações, mas também **contexto e justificativa** para cada obra.

---

## 🎯 Objetivos do projeto
- Demonstrar o uso de **agentes personalizados** no Azure AI Foundry.  
- Criar um agente capaz de **consultar uma base de dados literária** e responder de forma fiel e estruturada.  
- Apoiar **vestibulandos e estudantes** com recomendações que ampliem repertório sociocultural.  
- Mostrar como enriquecer a experiência do usuário com **campos adicionais** (complexidade e motivo para ler).  

---

## 🚀 Funcionalidades
- Recomenda livros por gênero literário.  
- Retorna **exatamente 3 indicações** por solicitação.  
- Usa **somente a base de dados fornecida** (sem buscas externas).  
- Reproduz fielmente a **sinopse original**.  
- Acrescenta **complexidade da leitura** e **motivo para ler**.  
- Contextualiza a resposta com uma introdução e um encerramento.  

---

## 🛠️ Processo de Criação
📌 Veja [como o agente foi desenvolvido](docs/processo.md) com imagens e explicações detalhadas.

---

## 🛠️ Tecnologias utilizadas
- **Azure AI Foundry** (Playground e configuração de agente)  
- **Modelo GPT-4.1**  
- **Base de dados em formato txt** com 200 livros  

---

## 📂 Estrutura do repositório
```
agente-bibliotecario/
│
├── Base_de_Dados.csv
├── README.md
 └── prints/
 ├── configuracao/ # prints da tela de configuração do agente
 ├── testes/ # prints das respostas durante os testes
 └── resultados/ # prints finais com respostas completas e corretas
```

---

## 💬 Exemplos de uso

### Pergunta: Quais livros clássicos você recomenda para o ENEM?
Clássicos da literatura são ótimos para quem se prepara para o ENEM, pois ampliam repertório e ajudam na compreensão de temas recorrentes. Veja três sugestões:

**1. Dom Quixote — Miguel de Cervantes**  
- Sinopse: "Um fidalgo espanhol enlouquece lendo romances de cavalaria e decide se tornar um cavaleiro andante para restaurar a justiça no mundo, acompanhado de seu fiel Sancho Pança."  
- Complexidade: Intermediário  
- Motivo para ler: Marca o início do romance moderno e satiriza a literatura de cavalaria.  

**2. Vidas Secas — Graciliano Ramos**  
- Sinopse: "A saga da família de retirantes nordestinos em sua luta por sobrevivência contra a seca e a miséria do sertão."  
- Complexidade: Iniciante  
- Motivo para ler: Retrato brutal da seca nordestina e da desumanização pela miséria.  

**3. Crime e Castigo — Fiódor Dostoiévski**  
- Sinopse: "Um estudante pobre comete um assassinato motivado por teorias morais e enfrenta as consequências de seu ato."  
- Complexidade: Intermediário  
- Motivo para ler: Explora dilemas universais de culpa, redenção e moralidade humana.  

---

### Pergunta: Tem sugestões de leitura para redação?
Uma boa escolha de livros pode ampliar repertório sociocultural, algo valorizado em provas como o ENEM. Veja três obras ideais:

**1. Quarto de Despejo — Carolina Maria de Jesus**  
- Sinopse: "O diário real de Carolina, catadora de papel, descreve a dura realidade da vida na favela do Canindé em São Paulo."  
- Complexidade: Iniciante  
- Motivo para ler: Documento vital da realidade social brasileira, escrito por uma voz marginalizada.  

**2. Vidas Secas — Graciliano Ramos**  
- Sinopse: "A saga da família de retirantes nordestinos em sua luta por sobrevivência contra a seca e a miséria do sertão."  
- Complexidade: Iniciante  
- Motivo para ler: Retrato brutal da seca nordestina e da desumanização pela miséria.  

**3. Ensaio sobre a Cegueira — José Saramago**  
- Sinopse: "Uma epidemia inexplicável de cegueira branca atinge uma cidade, expondo a natureza humana e a desintegração social."  
- Complexidade: Intermediário  
- Motivo para ler: Alegoria poderosa sobre moralidade, solidariedade e fragilidade social.  

---

## 📊 Monitoramento e Avaliação do Agente

Durante os testes e validações do agente bibliotecário, foram capturadas imagens dos dashboards do Microsoft Foundry que mostram o desempenho, uso e qualidade das respostas. Abaixo estão as explicações de cada uma:

### 🖼️ 1. Avaliação de Execuções (aba "Evaluation")
- Exibe gráficos sobre as **execuções do agente** entre os dias 11/11 e 14/11.
- Mostra quantas execuções foram concluídas ou falharam, além do uso de **tokens** (texto processado).
- Ajuda a entender o volume de uso e se houve falhas técnicas.

### 🖼️ 2. Monitoramento de Chamadas e Erros (aba "Monitor")
- Mostra o número de **chamadas e execuções** do agente entre 13/11 e 16/11.
- Apresenta a **taxa de erro** (0.08 em 16/11), indicando estabilidade.
- Inclui critérios de avaliação como **correção, relevância, confiabilidade e ética**.

### 🖼️ 3. Histórico de Conversas (aba "Traces")
- Lista todas as **conversas realizadas com o agente** entre 12/11 e 19/11.
- Mostra status, tempo, tokens usados, custo estimado e versão do agente.
- Útil para rastrear interações e verificar se foram concluídas corretamente.

### 🖼️ 4. Visão Geral do Monitoramento (aba "Monitor")
- Painéis com métricas gerais de uso (208.9k), avaliações e sugestões automáticas.
- Permite agendar avaliações e receber recomendações para melhorar o desempenho.
- Ideal para acompanhar o projeto de forma estratégica e contínua.

---

## 📖 Aprendizados e Desafios

### 🔍 Aprendizados
- **Importância das instruções claras**: o agente responde corretamente quando as *Instructions* são bem detalhadas.
- **Uso fiel da base de dados**: garantir que o agente não invente informações trouxe consistência.
- **Valor dos campos adicionais**: complexidade e motivo para ler tornaram as recomendações mais úteis.
- **Contextualização nas respostas**: introduções e encerramentos deixaram as respostas mais completas.

### ⚡ Desafios
- **Equilibrar simplicidade e riqueza**: ajustar as instruções para evitar respostas secas.
- **Estruturação da base de dados**: manter consistência ao adicionar novas colunas.
- **Testes com diferentes públicos**: adaptar respostas para vestibulandos e leitores iniciantes.
- **Limitação de 3 livros por vez**: reforçar essa regra nas instruções para evitar respostas longas demais.

### 🎯 Conclusão
O projeto mostrou como é possível criar um agente literário que vai além de simples recomendações, oferecendo **curadoria inteligente** e **apoio real para estudantes e leitores**.

---

## 📌 Como testar
1. Abra o agente no **Azure AI Foundry**.  
2. Vá para a aba **Playground**.  
3. Faça perguntas como:  
   - “Quais livros de ficção científica você recomenda?”  
   - “Me indique romances clássicos.”  
   - “Quero leituras fáceis para redação.”  
4. O agente retornará **3 livros com título, sinopse, complexidade e motivo para ler**.  

---

## 🔗 Links úteis
- [Azure AI Foundry](https://ai.azure.com)  
- [Documentação do Foundry](https://learn.microsoft.com/azure/ai-studio/)  
