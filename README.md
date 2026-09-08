# 📚 Miniguia de Estudos: Engenharia de Prompt e Otimização para LLMs

Projeto desenvolvido como desafio prático da plataforma **DIO**, focado no uso do **NotebookLM** como ferramenta de aprendizagem ativa, curadoria de conhecimento e engenharia de prompt.

---

## 🎯 Contexto e Objetivos

- **Tema Escolhido:** Engenharia de Prompt e Otimização de Comandos para LLMs
- **Contexto:** Estudo das melhores técnicas, padrões de escrita (_prompt patterns_) e estratégias de instrução para extrair respostas mais precisas, estruturadas e úteis de modelos de linguagem (como ChatGPT, Gemini e NotebookLM).
- **Objetivos de Estudo:**
  1. Compreender a anatomia de um prompt de alta performance (Role, Context, Instruction, Constraint, Output Format).
  2. Testar e documentar técnicas como _Few-Shot Prompting_, _Chain-of-Thought_ (Cadeia de Pensamento) e definição de personas.
  3. Mapear alucinações/erros comuns e como evitá-los através de restrições de contexto.

---

## 📚 Curadoria de Fontes

Fontes abertas selecionadas e utilizadas para alimentação e consulta no NotebookLM:

1. **Prompt Engineering Guide (DAIR.AI)** – [https://www.promptingguide.ai/pt](https://www.promptingguide.ai/pt) (Guia completo sobre técnicas de prompting).
2. **Documentação Oficial de Engenharia de Prompt da OpenAI** – [https://platform.openai.com/docs/guides/prompt-engineering](https://platform.openai.com/docs/guides/prompt-engineering) (Boas práticas de estruturação).
3. **Anthropic Prompt Engineering Interactive Tutorial** – [https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/overview) (Técnicas focadas em clareza e estrutura).

---

## 🧪 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

### Comparativo de Prompts

- **Prompt Inicial (Genérico / Superficial):**

  > _"Como faço para criar um prompt bom?"_
  - **Resultado:** Resposta ampla, genérica e teórica, listando apenas dicas básicas sem estrutura prática.

- **Prompt Refinado (Estratégico / Com Restrições):**
  > _"Atue como um Especialista em Engenharia de Prompt. Explique a técnica 'Chain-of-Thought' (Cadeia de Pensamento). Estruture sua resposta em 3 partes: 1) Definição simples; 2) Quando utilizar; 3) Um exemplo prático comparando um prompt direto contra um prompt usando Chain-of-Thought. Responda em formato Markdown."_
  - **Resultado:** Resposta rica, estruturada, didática e pronta para uso imediato.

### Cicatrizes & Aprendizados

- **Problema:** Respostas prolixas ou com alucinações de conteúdo.
- **Causa:** Ausência de restrições de escopo (_constraints_) e indefinição do formato de saída.
- **Solução:** Definir _personas_ claras, delimitar o contexto estritamente às fontes fornecidas e exigir formatos rígidos de saída (tabelas, tópicos ou JSON).

---

## 📖 Miniguia de Estudo

### 📌 Resumo Estruturado

A Engenharia de Prompt é a disciplina de estruturar textos de entrada para direcionar LLMs a gerarem respostas precisas. O arcabouço essencial para um prompt de alta performance conta com:

1. **Atribuição de Papel (Role):** Define quem a IA deve simular.
2. **Contexto (Context):** Informações de fundo para balizar a resposta.
3. **Instrução Clara (Instruction):** O comando direto e objetivo.
4. **Restrições (Constraints):** Limites de escopo, tom e tamanho.
5. **Formato de Saída (Output):** Organização visual (Markdown, Tabela, JSON).

### 📖 Glossário de Conceitos

- **Zero-Shot Prompting:** Instruir a IA sem fornecer exemplos prévios.
- **Few-Shot Prompting:** Fornecer exemplos no prompt para ensinar o padrão esperado.
- **Chain-of-Thought (CoT):** Induzir a IA a resolver problemas passo a passo.
- **Persona/Role:** Atribuir um papel ou perfil profissional ao modelo.
- **Hallucination (Alucinação):** Geração de informações falsas apresentadas com convicção.
- **System Prompt:** Diretrizes primárias que definem o comportamento global da IA.

### 🛠️ Prompts Reutilizáveis

- **Para Aprendizado Ativo:** `"Explique o conceito de [CONCEITO] como se eu tivesse 10 anos. Em seguida, faça 3 perguntas para testar minha compreensão."`
- **Para Engenharia Reversa:** `"Analise a resposta abaixo e crie o prompt ideal que teria gerado esse resultado exato:"`
- **Para Síntese:** `"Resuma o texto abaixo em uma tabela com 3 colunas: Conceito, Aplicação Prática e Cuidados. Texto: [COLE O TEXTO AQUI]"`
