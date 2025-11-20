# 📚 Bibliotecário Virtual

Agente bibliotecário digital desenvolvido no **Microsoft Foundry**, com foco em recomendações literárias educativas.  
O agente consulta exclusivamente uma base de dados própria e sugere livros de acordo com os interesses do usuário.

---

## 📑 Índice

- [Descrição do projeto](#descrição-do-projeto)
- [Documentação](#documentação)
- [Objetivo](#objetivo)
- [Ferramentas utilizadas](#ferramentas-utilizadas)
- [Prints e evidências](#prints-e-evidências)
- [Referências externas](#referências-externas)
- [Estrutura de diretórios](#estrutura-de-diretórios)
- [Conclusão](#conclusão)

---

## 📄 Descrição do projeto

Este repositório documenta todas as etapas de criação, configuração e testes do agente bibliotecário digital.  
Ele foi pensado para ser **educativo, transparente e reprodutível**, servindo como referência para projetos semelhantes.

---

## 🧭 Documentação

- 🛠️ [Como foi feito](docs/como-foi-feito.md)  
  Explica o processo de criação do agente dentro do Foundry.

- ⚙️ [Configuração](docs/configuracao.md)  
  Detalhes técnicos sobre modelo, ferramentas, instruções e parâmetros utilizados.

- 🧱 [Arquitetura](docs/arquitetura.md)  
  Esquema da arquitetura do agente, mostrando camadas e conexões.

- 📜 [Prompts](docs/prompts.md)  
  Lista completa das instruções e starter prompts configurados para o agente.

- 📚 [Bases de conhecimento](docs/bases.md)  
  Documentação das bases de dados utilizadas.  
  ➡️ Arquivos disponíveis na pasta [`bases`](bases)

- 🧪 [Testes](docs/testes.md)  
  Evidências dos testes realizados durante o desenvolvimento.

- 📸 [Resultados](docs/resultados.md)  
  Exemplos de respostas finais do agente após ajustes.

---

## 🚀 Objetivo

O agente foi criado para:
- Recomendar **exatamente 3 livros** por vez  
- Informar o usuário caso o tipo de livro não esteja na base  
- Utilizar **apenas a base de dados** anexada  
- Para cada livro, fornecer:
  - Título  
  - Autor  
  - Ano  
  - Sinopse  
  - Complexidade da leitura  
  - Motivo para ler  

---

## 🧰 Ferramentas utilizadas

- **Microsoft Foundry**  
  Ambiente de desenvolvimento onde o agente foi criado e configurado.

- **File Search**  
  Ferramenta ativada para permitir que o agente consulte diretamente os arquivos anexados.

- **Playground (Chat, YAML, Code)**  
  Utilizado para testar o comportamento do agente e ajustar instruções.

---

## 🖼️ Prints e evidências

Imagens de configuração, testes e resultados estão disponíveis na pasta [`prints`](prints), organizadas por etapa:

- [`prints/configuracao`](prints/configuracao)  
- [`prints/testes`](prints/testes)  
- [`prints/resultados`](prints/resultados)

---

## 🔗 Referências externas

- [Microsoft Foundry](https://foundry.microsoft.com)

---

## 📂 Estrutura de diretórios

```
bibliotecario-virtual/
├── bases/ # Arquivos da base de dados
├── docs/ # Documentação (como-foi-feito, configuração, arquitetura, prompts, testes, resultados, bases)
├── prints/ # Imagens de configuração, testes e resultados
└── README.md # Página inicial do projeto
```
---

## ✅ Conclusão

Este repositório documenta todas as etapas de criação, configuração e testes do agente bibliotecário digital.  
Ele foi pensado para ser **educativo, transparente e reprodutível**. Toda a lógica de recomendação é baseada em uma base de dados própria, sem uso de fontes externas.

