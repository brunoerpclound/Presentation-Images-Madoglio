---
name: presentation-images-madoglio
description: Converte apresentações PDF, PPT/PPTX ou HTML em uma imagem por página ou slide, com opção de conversão fiel ou redesign hiperpersonalizado usando ChatGPT Images. Use quando o usuário quiser transformar uma apresentação inteira em imagens individuais, adaptar proporção, aplicar logo, substituir fundos ou reposicionar textos.
---

# Presentation Images Madoglio

Produza uma imagem final por página, slide ou tela lógica, preservando a ordem e o conteúdo factual da apresentação. Use o gerador de imagens disponível no ambiente (ChatGPT Images; a versão oferecida pelo produto, quando indicada como ChatGPT Images 2.0) para criação e edição visual. Não afirme que uma versão específica está disponível sem confirmação do ambiente.

## Entrada

Aceite PDF, PPT/PPTX e HTML. Se nenhum arquivo ou URL acessível tiver sido fornecido, solicite-o antes de executar. Para HTML, confirme a unidade de saída somente se ela não estiver evidente: páginas/telas já delimitadas ou seções principais. Não divida uma página contínua arbitrariamente sem avisar.

Inspecione o arquivo para contar as unidades, extrair os textos e identificar dimensões, imagens e elementos recorrentes. Informe ao usuário quantas imagens serão produzidas. Se o arquivo estiver protegido, corrompido, incompleto ou depender de recursos remotos inacessíveis, explique o bloqueio e peça uma entrada utilizável.

## Entrevista obrigatória

Faça perguntas curtas e com opções selecionáveis quando a interface permitir. Aproveite respostas já fornecidas e não repita perguntas. Agrupe no máximo três perguntas por rodada.

1. Pergunte o formato final: `16:9`, `9:16` ou `1:1`.
2. Pergunte se deve aplicar uma logo.
   - Se sim, solicite o arquivo da logo, uma URL pública direta ou um link acessível do Google Drive. Aceite PNG/SVG com transparência como preferência; peça posição e tamanho apenas se não puder inferi-los com segurança.
   - Se não, prossiga.
3. Pergunte se deve trocar as imagens de fundo.
   - Se sim, peça uma descrição do estilo, assunto, cores e restrições. Quando útil, ofereça manter uma direção visual única em toda a série.
   - Se não, preserve os fundos originais.
4. Pergunte se os textos devem permanecer exatamente na mesma posição.
   - Se sim, preserve posição, hierarquia e tamanho relativo. Não apresente opções de reposicionamento.
   - Se não, faça as duas perguntas curtas abaixo, permitindo combinar tamanho e posição de forma independente.

### Opções de texto

**1. Qual tamanho deseja?**

- Menor
- Igual ao original
- Maior

**2. Em qual posição devem ficar?**

- Posição original
- Topo
- Centro
- Inferior

Registre as duas escolhas e aplique a combinação a todos os slides, preservando a hierarquia entre título, subtítulo e corpo. Se o usuário escolher `Igual ao original` e `Posição original`, trate como preservação integral do layout textual.

Antes de iniciar, apresente um resumo compacto das escolhas. Não peça nova confirmação se todas as respostas forem inequívocas e a execução não exigir ação externa sensível.

## Escolha do modo

- **Conversão fiel:** quando não houver troca de fundo, logo nova, mudança de proporção com recomposição ou alteração do texto. Renderize diretamente cada unidade; não passe a imagem pelo gerador apenas para converter formato.
- **Redesign com IA:** quando houver criação ou substituição visual. Use o gerador para fundos e elementos visuais, mas componha textos e logos por meios determinísticos sempre que possível. Isso reduz erros de ortografia, números e marcas.

Para instruções completas de composição, tratamento por formato e controle de qualidade, leia [references/workflow.md](references/workflow.md).

## Regras essenciais

- Preserve integralmente textos, números, datas, nomes próprios, URLs e ordem dos slides, salvo pedido explícito de edição textual.
- Nunca invente conteúdo ausente nem redesenhe uma marca com IA quando o arquivo original da logo estiver disponível.
- Não distorça ou corte conteúdo importante ao adaptar a proporção. Prefira recomposição, expansão de fundo ou margens coerentes.
- Trate cada slide como parte da mesma identidade visual; mantenha paleta, tipografia, margens e estilo consistentes.
- Não exponha imagens de referência ou ativos privados em serviços externos sem autorização e sem que o ambiente permita.
- Se a legibilidade entrar em conflito com a posição escolhida, preserve o conteúdo e faça o menor ajuste necessário, explicando-o na entrega.

## Entrega

Entregue arquivos individuais em PNG por padrão, numerados com zeros à esquerda: `slide-01.png`, `slide-02.png`, etc. Se o usuário pedir JPG/WebP, use o formato solicitado. Inclua também um ZIP com todas as imagens quando houver mais de uma unidade, sem substituir os arquivos individuais.

Antes de entregar, verifique contagem, ordem, dimensões, legibilidade, fidelidade textual, consistência visual, aplicação correta da logo e ausência de cortes. Informe resumidamente o total, a proporção, o modo usado e qualquer limitação real.
