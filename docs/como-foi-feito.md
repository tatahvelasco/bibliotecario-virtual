# 🛠️ Como o agente foi desenvolvido

Este documento apresenta o passo a passo da criação do agente bibliotecário digital no Microsoft Foundry, com imagens e explicações de cada etapa.

---

## 1. Acesso ao ambiente Foundry

O projeto foi iniciado na plataforma [Microsoft Foundry](https://ai.azure.com), onde foi criado um novo agente a partir do botão **Start building → Create agent**.

📷 *Imagem: Tela de boas-vindas com opções de criação de agente*

---

## 2. Criação do agente

Foi definido um nome único para o agente (`gpts-talitavelasco`) e iniciado o processo de configuração.

📷 *Imagem: Modal de criação do agente com campo de nome preenchido*

---

## 3. Configuração inicial

Na aba **Agents**, foram ajustadas as configurações principais:

- Modelo selecionado: `gpt-4-1`
- Ferramentas ativadas: `File search`
- Instruções personalizadas para limitar o escopo e garantir respostas fiéis à base.

📷 *Imagem: Tela de configuração do agente com modelo e ferramentas visíveis*

---

## 4. Adição de ferramentas

A ferramenta **File search** foi adicionada para permitir que o agente consultasse diretamente a base de dados textual.

📷 *Imagem: Seleção da ferramenta File search e botão de confirmação*

---

## 5. Upload da base de dados

A base de dados (`Base de Dados.txt`) foi anexada a um índice vetorial chamado `base-de-dados-completa`.  
Posteriormente, versões melhoradas da base foram adicionadas para refinar as respostas.

📷 *Imagem: Tela de upload e anexação da base com status de sucesso*

---

## 6. Playground e testes

No Playground, o agente foi testado com diferentes perguntas. A base foi trocada e ajustada conforme os testes evoluíam.  
O agente foi configurado para responder com 3 livros por vez, incluindo sinopse, complexidade e motivo para ler.

📷 *Imagem: Tela do Playground com base ativa e ferramenta em uso*

---

## 7. Instruções refinadas

As instruções foram ajustadas para garantir que o agente:

- Perguntasse sobre ficção ou não ficção.
- Solicitasse o gênero desejado.
- Retornasse **exatamente 3 livros** com sinopse fiel, complexidade e motivo para ler.
- Usasse linguagem natural e acessível.

📷 *Imagem: Instruções detalhadas no painel do agente*

---

## 8. Versões e variações

Foram criadas versões alternativas do agente (`dlg-bibliotecario`, `afg-bibliotecario`) com variações nas instruções, prompts iniciais e estilo de resposta.  
Cada versão foi testada com diferentes bases e configurações.

📷 *Imagem: Configuração de versões com prompts e descrição personalizada*

---

## 9. Monitoramento e avaliação

O desempenho do agente foi acompanhado por meio dos dashboards do Foundry:

- Número de execuções
- Taxa de erro
- Histórico de conversas
- Uso de tokens

📷 *Imagens: Painéis de monitoramento e avaliação com gráficos e métricas*

---

## ✅ Conclusão

O agente foi configurado com foco em **clareza, fidelidade à base e utilidade para estudantes**.  
As imagens acima documentam todas as etapas, desde a criação até os testes finais, garantindo transparência e qualidade no desenvolvimento.

---

🔗 Voltar para o [README principal](../README.md)

