# Fluxo de produção e controle de qualidade

## 1. Preparação por formato

### PDF

Renderize cada página em alta resolução e preserve transparências e vetores quando a ferramenta permitir. Use a numeração do PDF como ordem canônica.

### PPT/PPTX

Renderize os slides com um motor compatível com PowerPoint/LibreOffice. Inspecione fontes ausentes, mídia, animações e elementos fora da tela. A saída representa o estado estático principal de cada slide; avise se animações contiverem informação que não aparece nesse estado.

### HTML

Abra com viewport correspondente à proporção escolhida. Aguarde fontes e imagens carregarem. Identifique páginas, rotas, seções ou contêineres de slide já definidos. Para uma página longa sem divisões claras, peça ao usuário como segmentar.

## 2. Dimensões recomendadas

Use, salvo requisito diferente:

| Proporção | Tamanho recomendado |
| --- | --- |
| 16:9 | 1920 × 1080 px |
| 9:16 | 1080 × 1920 px |
| 1:1 | 1080 × 1080 px |

Mantenha a mesma dimensão em toda a série.

## 3. Conversão fiel

Renderize a origem diretamente. Se a proporção de destino diferir, use uma destas estratégias, nesta ordem:

1. ampliar ou estender o fundo sem alterar o conteúdo;
2. recompor blocos mantendo hierarquia e leitura;
3. inserir margens coerentes com a identidade visual.

Evite recorte de texto, logo, rosto ou elemento informativo.

## 4. Redesign com IA

Crie primeiro uma direção visual comum e reutilize-a nos slides. Ao gerar fundos, peça áreas de respiro adequadas ao posicionamento escolhido para o texto. Gere ou edite visuais sem texto embutido sempre que possível.

Monte depois, de forma determinística:

- textos extraídos da origem;
- logo original fornecida;
- formas, linhas, numeração e elementos gráficos que exigem precisão;
- rodapés, URLs e chamadas para ação.

Se for inevitável gerar texto dentro da imagem, confronte-o visualmente com o texto extraído e refaça qualquer slide com erro.

## 5. Logo

Use o arquivo original em vez de pedir ao modelo para recriá-lo. Preserve proporção, cores e área de proteção. Garanta contraste; se necessário, use somente um fundo discreto ou uma variante oficial fornecida pelo usuário. Não invente uma versão monocromática ou altere a marca sem autorização.

## 6. Texto e layout

“Mesma posição” significa preservar âncora, alinhamento, ordem e hierarquia, admitindo apenas ajustes mínimos para caber na nova proporção. “Topo”, “centro” e “parte inferior” indicam a zona principal do bloco textual, não alinhamento rígido de todos os elementos.

Ao alterar tamanho, mantenha contraste, entrelinha, margens seguras e hierarquia entre título, subtítulo e corpo. Não aplique um único tamanho a todo o texto.

## 7. Revisão obrigatória

Compare cada saída com a unidade original e verifique:

- quantidade e sequência;
- dimensões e orientação;
- textos completos e sem erros;
- números, datas, nomes e URLs;
- logo correta, nítida e consistente;
- ausência de cortes e sobreposições;
- estilo coerente entre todas as imagens;
- imagens sem artefatos ou conteúdo inadequado.

Corrija falhas antes da entrega. Para apresentações longas, uma folha de contato pode auxiliar a revisão, mas não substitui a inspeção individual.

## 8. Estrutura de saída

Organize a entrega em uma pasta com nomes ordenáveis:

```text
nome-da-apresentacao-imagens/
├── slide-01.png
├── slide-02.png
└── nome-da-apresentacao-imagens.zip
```

Não inclua arquivos temporários, renders intermediários ou ativos privados no ZIP.
