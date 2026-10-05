<div align="center">

# GuiaCiber

**Cibersegurança explicada para quem está começando.**

![Python](https://img.shields.io/badge/Python-3776ab?style=flat-square) ![HTML · CSS · JavaScript](https://img.shields.io/badge/HTML%20%C2%B7%20CSS%20%C2%B7%20JavaScript-2563eb?style=flat-square) ![Projeto DIO](https://img.shields.io/badge/Projeto%20DIO-8257e5?style=flat-square)

</div>

---

Assistente educacional que responde perguntas sobre segurança digital usando uma base de conhecimento local e correspondência de palavras-chave. Desenvolvido para o desafio **Construa seu Assistente Virtual com Inteligência Artificial**, da DIO.

> O protótipo atual não usa um modelo generativo nem uma API de IA. Seu foco é documentar e demonstrar o comportamento de um assistente.

## Explore os temas

Senhas, MFA, phishing, engenharia social, OSINT, metadados, DevSecOps e sistemas operacionais.

## Experimente

### No navegador

Abra [src/index.html](src/index.html). Essa versão funciona sem instalação.

### No terminal

Com Python 3.10 ou superior:

```bash
python src/assistente.py
```

Pergunte **“Como identificar phishing?”** ou **“Por que usar MFA?”**. Digite `sair` para encerrar.

## Como a resposta é construída

1. A pergunta é normalizada.
2. Palavras-chave são comparadas com os tópicos disponíveis.
3. O tópico encontrado fornece a resposta-base.
4. Sem correspondência suficiente, o assistente informa a limitação.

## Mapa do projeto

| Arquivo | Conteúdo |
| --- | --- |
| [Base de conhecimento](data/base_conhecimento.json) | Tópicos, palavras-chave e respostas. |
| [Agente](docs/agente.md) | Objetivo, público e comportamento. |
| [Prompts](docs/prompts.md) | Instruções e regras de segurança. |
| [Avaliação](docs/avaliacao_metricas.md) | Critérios e resultados esperados. |
| [Perguntas de teste](tests/perguntas_teste.md) | Roteiro de avaliação manual. |
| [Pitch](docs/pitch.md) | Problema, solução e proposta de valor. |

## Limitações e evolução

A base é pequena e a busca não é semântica. O assistente não faz diagnóstico técnico. Possíveis próximos passos incluem ampliar os tópicos, implementar busca semântica e avaliar uma integração generativa com credenciais mantidas no servidor.

## Uso seguro

Use perguntas fictícias ou genéricas. Não insira senhas, chaves de API ou dados pessoais. As respostas são material educacional e precisam ser avaliadas no contexto de uso.
