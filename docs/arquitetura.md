# 🧱 Arquitetura do Agente Bibliotecário

Este documento apresenta a arquitetura do agente bibliotecário digital criado na plataforma Microsoft Foundry. A estrutura foi pensada para garantir clareza, modularidade e eficiência na recomendação de livros.

---

## 🧭 Visão geral da arquitetura

A arquitetura é composta por camadas que se conectam da seguinte forma:

1. **Ambiente de desenvolvimento**
   - Plataforma: Microsoft Foundry

2. **Projeto**
   - Nome: `project-frontier-girls`

3. **Agente**
   - Identificador: `afg-bibliotecario`
   - Criado via interface de criação de agentes

4. **Modelo**
   - Versão utilizada: `GPT-4.1`
   - Escolhido por sua capacidade de gerar respostas contextualizadas e bem estruturadas

5. **Ferramentas ativadas**
   - `File search`: permite ao agente consultar diretamente os arquivos anexados
   - Nenhuma outra fonte de pesquisa foi habilitada

6. **Base de dados**
   - Arquivos anexados:
     - `Base de Dados.txt`
     - `Base de Dados Melhorada.txt`
   - Indexados para uso exclusivo do agente

7. **Instruções refinadas**
   - Recomendar **exatamente 3 livros** por vez
   - Informar o usuário **caso o tipo de livro não esteja na base**
   - Utilizar **apenas a base de dados** (sem outras fontes)
   - Para cada livro, fornecer:
     - Título
     - Autor
     - Ano
     - Sinopse
     - Complexidade da leitura
     - Motivo para ler

8. **Playground para testes**
   - Utilizado para validar respostas e ajustar instruções
   - Testes realizados com variações de estilo e tom

---

## ✅ Conclusão

A arquitetura foi desenhada para garantir que o agente funcione de forma confiável, educativa e alinhada com os objetivos do projeto.  
Cada componente — do modelo à base de dados — contribui para uma experiência de recomendação literária clara, útil e personalizada.
