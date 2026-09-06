# Presentation Images Madoglio

Skill para converter apresentações em PDF, PPT/PPTX ou HTML em imagens individuais por página ou slide. Permite conversão fiel e redesign visual com IA, preservando textos, dados e ordem da apresentação.

## Instalação no Codex

Clone ou copie este repositório para a pasta de Skills da conta, preservando a estrutura de arquivos.

```text
~/.codex/skills/presentation-images-madoglio/
├── SKILL.md
├── agents/openai.yaml
└── references/workflow.md
```

Em instalações padrão no Windows, a pasta de Skills fica em `%USERPROFILE%\.codex\skills`. Em ambientes com `CODEX_HOME` configurado, use `$CODEX_HOME/skills/presentation-images-madoglio`.

Exemplo com Git:

```bash
git clone https://github.com/brunoerpclound/Presentation-Images-Madoglio.git ~/.codex/skills/presentation-images-madoglio
```

Inicie uma nova conversa no Codex após a instalação.

## Uso

Invoque a Skill pelo nome:

```text
$presentation-images-madoglio
```

Exemplo: “Use `$presentation-images-madoglio` para converter esta apresentação em imagens 16:9, preservando o layout e os textos.”

## Outros harnesses compatíveis

Em qualquer harness que suporte o padrão `SKILL.md`, copie a pasta inteira para o diretório de Skills configurado por esse ambiente. O arquivo `SKILL.md` contém as instruções portáveis; `agents/openai.yaml` oferece metadados de interface para ambientes compatíveis com o Codex.
