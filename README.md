# Feito In 3D Maker

Versão pronta para GitHub Pages.

## Arquivos

- `index.html`: ferramenta completa em HTML, CSS e JavaScript.

## Atualizações desta versão

- Exportação em GIF, MP4 e MOV.
- Opção de formato da tela:
  - Vertical Full HD 9:16
  - 4:3 clássico
- Controle separado entre velocidade do movimento e duração final do arquivo.
- Três opções de qualidade de exportação:
  - Leve / rápido
  - Padrão
  - Alta qualidade
- Resoluções por formato:
  - Vertical: 540×960, 720×1280 ou 1080×1920
  - 4:3: 640×480, 960×720 ou 1440×1080
- Correção no carregamento do GIF usando worker em Blob para evitar travamento comum com worker externo.
- Botão de download na lateral e sobre o preview após exportar.

## Publicação no GitHub Pages

1. Suba o `index.html` na raiz do repositório.
2. Vá em Settings > Pages.
3. Escolha Deploy from a branch.
4. Selecione a branch `main` e a pasta `/root`.
5. Salve e aguarde o link do GitHub Pages.

## Observação

GIF em alta qualidade pode gerar arquivos muito pesados. Para vídeos longos, MP4 costuma ser mais leve e mais estável.


## Atualização de navegação

Os botões Exportar, Limpar alinhamento, Limpar tudo e Baixar arquivo ficam na coluna direita, abaixo do visualizador, para facilitar o fluxo de uso.


## Ajuste mobile

Na versão mobile, o preview aparece acima da área de carregamento da foto para facilitar a visualização do resultado antes dos controles.

## Atualização — controle de exposição

Adicionada uma barra de Exposição / luz da imagem logo abaixo da intensidade do efeito de cor. O ajuste aparece no preview e também é aplicado no GIF, MP4 ou MOV exportado.


## Atualização — Foto Horizontal e Foto Vertical

A ferramenta agora aceita dois tipos de imagem de entrada:

- Foto Horizontal: quadros lado a lado.
- Foto Vertical: quadros empilhados.

O seletor fica no grupo "Carregamento e ajuste de ponto". O restante da ferramenta continua usando o mesmo fluxo de alinhamento, efeitos, exposição, RGB, marca d'água, ajuste fino e exportação em GIF, MP4 ou MOV.

## Atualização — Exportação horizontal

A ferramenta agora também exporta em:

- Horizontal Full HD — 1920 × 1080
- Horizontal 4K — 3840 × 2160

Essas opções ficam no seletor "Formato da tela". A orientação da foto de entrada continua independente do formato final exportado.


## Atualização — Sinal visual de ponto automático

Ao clicar em Selecionar pontos automáticos, o preview escurece levemente e exibe uma mira pulsante com instrução para o usuário clicar no ponto principal da imagem. O aviso desaparece quando o mouse entra no preview ou ao tocar/clicar na área.

## Atualização — Ajuste fino e aviso de ponto

- A guia de ajuste fino agora abre minimizada por padrão.
- O aviso visual para clicar no ponto automático aparece somente na primeira vez que o usuário usa esse recurso no navegador.

## Atualização — JPG alto e botão de compra

- Adicionado botão "Exportar JPG alto" na área de ações do arquivo.
- O JPG é gerado em alta qualidade, usando o formato de tela selecionado.
- Adicionado botão "Compre sua lente" no cabeçalho, apontando para a página do produto no Mercado Livre.
- Depois que o primeiro ponto é marcado e os pontos automáticos são sugeridos, o botão "Aplicar pontos" pisca para indicar a próxima ação.

## Atualização — Nitidez

Adicionada a opção "Nitidez da imagem" na aba Ajustes criativos. A barra vai de 0% a 100% e ajuda a recuperar definição quando a foto está levemente desfocada. O ajuste aparece no preview e também no GIF, MP4, MOV e JPG exportados.


## Atualização — Glow

Adicionada a opção "Glow / luz dos sonhos" na aba Ajustes criativos. A barra vai de 0% a 100% e cria um brilho suave nos pontos de luz da imagem, dando um aspecto mais sonhador. O ajuste aparece no preview e também no GIF, MP4, MOV e JPG exportados.

## Atualização — LUT personalizado

Adicionada a opção de carregar LUT personalizado na aba Ajustes criativos. O usuário pode carregar arquivos .CUBE ou .3DL e o LUT é aplicado no preview e nos arquivos exportados em GIF, MP4, MOV e JPG alto.


## Atualização — Intensidade do LUT

O controle de intensidade do efeito agora também atua sobre o LUT personalizado, permitindo misturar o visual original com o LUT carregado de forma mais suave ou mais intensa.


## Atualização — Controle manual de enquadramento

Depois que os pontos são aplicados, o usuário pode ajustar o enquadramento diretamente no preview: arrastando com o mouse para reposicionar a imagem e usando o scroll para dar zoom ou tirar zoom. Esse ajuste afeta o preview e também a exportação final.

## Atualização — Enquadramento manual no mobile

O controle manual de enquadramento agora também funciona no mobile:
- 1 dedo para mover a imagem;
- 2 dedos em pinça para dar zoom ou tirar zoom.

A versão desktop continua usando mouse para mover e scroll para zoom.

## Atualização — Botões de download

Adicionados botões de destaque no rodapé para baixar a versão desktop:

- Windows: https://drive.google.com/uc?export=download&id=1oNmfnYf6lIPkR9rqdCOs4RryNkkGTEJN
- Mac: https://drive.google.com/uc?export=download&id=1ToLK8iyH-6f2GxnzdFk3xFON8Mcpg4bO

Os botões aparecem acima do crédito do desenvolvedor e usam ícones SVG desenhados para cada sistema.


## Atualização — Link Mac

Link direto atualizado para Mac:

https://drive.google.com/uc?export=download&id=1ToLK8iyH-6f2GxnzdFk3xFON8Mcpg4bO

## Atualização — Interpolação de tempo e auxílio inteligente de pontos

### 1) Interpolação de tempo / quadros
Foi restaurado o recurso de interpolação na ferramenta de imagens.

- Controle em barra (`0%` a `100%`)
- Atua no preview e na exportação
- Funciona com GIF, MP4 e MOV
- Mantém o tempo total, alterando a suavidade com quadros intermediários

### 2) Auxílio inteligente de pontos
Foi adicionada uma opção chaveada para ajudar o usuário a escolher o melhor ponto inicial.

- Quando ativada, a ferramenta avalia o **1º frame**
- Mostra **pontos sugeridos** com base em detalhes fortes e fáceis de rastrear
- O usuário pode clicar em um dos pontos sugeridos
- Depois do clique, a ferramenta tenta mapear esse ponto nos outros frames e **já exibe o preview do GIF automaticamente**
- Se preferir, o usuário ainda pode clicar manualmente em qualquer detalhe da imagem

### Favicon
Mantenha também o arquivo `favicon.svg` na raiz do projeto para a guia personalizada com o símbolo de 3 lentes.

## Correção — Preview preto e clique nos pontos sugeridos

- Corrigido um erro na interpolação que fazia o preview ficar preto/travado após carregar a imagem.
- O preview agora volta a usar corretamente os frames base antes de criar os frames intermediários.
- No modo **Auxílio inteligente de pontos**, ao clicar em um ponto sugerido:
  - a ferramenta tenta mapear o ponto nos outros frames;
  - o preview do GIF já começa a rodar automaticamente;
  - o botão **Aplicar pontos** fica habilitado para confirmação.

## Atualização — Vídeo lateral direito com arquivo local leve

- Removido completamente o bloco incorporado do Instagram.
- Mantido apenas o vídeo local na lateral direita do preview.
- Substituído o vídeo anterior pelo arquivo mais leve: `assets/feitoin3d-kenji-lente-3d.mp4`.
- O vídeo roda em loop, autoplay e sem som por padrão.
- O usuário pode ativar/desativar o som pelo botão abaixo do vídeo.
- Na versão mobile, o vídeo lateral continua oculto.


## Atualização — UI refinada
- Reorganização visual da interface em fluxo de produção.
- Adicionado painel de status das 4 etapas: importar, alinhar, estilizar e exportar.
- Ajuste fino movido para acionamento por botão no painel esquerdo, evitando competição visual sobre o preview.
- Adicionado botão de resetar enquadramento.
- Bloco de exportação com resumo do resultado final.
- Adicionada a resolução Retrato 3:4.


## Atualização — Layout reestruturado
- Painel de ajustes permanece à esquerda e ocupa a primeira coluna.
- Fluxo de produção movido para a lateral direita, abaixo do vídeo demonstrativo.
- Vídeo lateral simplificado: sem textos, apenas vídeo em loop e botão de som.
- Exportar e baixar foi movido para dentro da aba recolhível de Exportar arquivo.
- Resolução 3:4 mantida.


## Ajustes finais de layout e padrão de exportação

- Vídeo lateral com opacidade reduzida por padrão e opacidade total no hover.
- Auxílio inteligente de pontos ativado por padrão.
- Botões “Selecionar pontos” e “Aplicar pontos” movidos para cima do preview.
- Ajuste fino voltou a ficar minimizado dentro do preview.
- “Resolução / formato da tela” movido para a primeira aba.
- Formato padrão alterado para MP4.
- Duração padrão de vídeo alterada para 10 segundos.
- Qualidade padrão alterada para Alta qualidade.


## Ajuste — Fluxo acima do vídeo e painéis recolhidos

- O painel **Fluxo de produção** foi movido para cima do vídeo na lateral direita.
- Os painéis laterais permanecem recolhidos mesmo após o carregamento da imagem.
- Apenas o primeiro painel fica aberto por padrão, até que o usuário decida minimizar ou abrir outro manualmente.
- Removida a abertura automática das abas de exportação e estilo após processar ou alinhar a imagem.


## Atualização — Otimização mobile

A versão mobile recebeu ajustes específicos de interface:
- cabeçalho mais compacto;
- cards e painéis mais enxutos;
- descrições longas dos painéis ocultas no mobile;
- botões maiores para toque;
- ações de pontos fixadas no topo da área de preview;
- preview com melhor aproveitamento vertical da tela;
- vídeo lateral continua oculto no mobile;
- área de exportação e frames adaptada para telas pequenas.


## Ajuste mobile — Preview e alinhamento no topo

Na versão mobile, a ordem visual foi ajustada para priorizar o uso prático:
- a área de preview aparece no topo;
- os botões **Selecionar pontos** e **Aplicar pontos** aparecem acima do preview;
- os painéis de configuração ficam abaixo, mantendo a versão desktop inalterada.

## Atualização — Links dos aplicativos desktop

Links atualizados no site:

- Windows: `https://drive.google.com/uc?export=download&id=1m9eM4IkeAane2aPNA4x5D2hir-yTX3a5`
- Mac: `https://drive.google.com/uc?export=download&id=1k7tsYe1P8lTQfpWx4LE553hIZwCY4vYQ`

Os links foram convertidos para formato de download direto do Google Drive.

## Atualização — Link Mac ZIP e aviso de instalação

- Link Mac atualizado para: `https://drive.google.com/uc?export=download&id=1K9m28_unAxTvaVusPPDWLBuzc0uiTtbY`
- Botão de Mac atualizado para **Baixar ZIP para Mac**.
- Adicionado pop-up antes do download do Mac.
- O pop-up informa que o macOS pode acusar arquivo danificado/corrompido por falta de assinatura Apple.
- O usuário precisa confirmar que leu o aviso antes de baixar o ZIP.


## Atualização — Tela inicial Lente 3D / Lente Retro

Foi adicionada uma tela inicial antes da ferramenta com duas opções:

- **Lente 3D**: mantém toda a lógica atual de montagem com múltiplos quadros, alinhamento, movimento, GIF, MP4, MOV e JPG.
- **Lente Retro**: transforma a página em um editor de foto focado em estética retrô/analógica.

### Modo Lente Retro

O modo Retro contém:
- painel de upload;
- painel de ajustes de imagem;
- recursos criativos reaproveitados da página 3D, como LUT personalizado, exposição, nitidez, glow, efeitos vintage e marca d'água;
- exportação focada em JPG alto;
- remoção/ocultação de recursos de GIF, movimento, alinhamento de múltiplos frames e interpolação.

### Suporte de arquivos

O seletor de arquivos da Lente Retro aceita JPG, PNG, WEBP, HEIC/HEIF, TIFF e extensões RAW comuns de câmera. Alguns formatos RAW dependem do suporte do navegador; quando não for possível abrir diretamente, o usuário deve converter para JPG, TIFF, PNG ou HEIC antes de editar.


## Correção — proporção dos painéis recolhíveis

Corrigida a proporção visual dos painéis laterais recolhíveis após a adição da tela inicial Lente 3D / Lente Retro.

- Painéis recolhidos voltam a ter altura compacta.
- Conteúdo interno fica totalmente oculto quando o painel está fechado.
- Títulos e descrições não ficam mais espremidos em faixas estranhas.
- Coluna esquerda recebeu leve ajuste de largura no desktop.


## Recursos novos para a Lente Retro

Com base nas referências visuais enviadas, o modo **Lente Retro** agora conta com recursos para facilitar resultados parecidos com ensaios analógicos / flash vintage:

### Receitas prontas
- **01 — Low light verde**
- **02 — Flash de festa**
- **03 — Golden retrô**
- **04 — Quarto nostálgico**

### Novos controles criativos
- **Temperatura / tom quente-frio**
- **Pretos desbotados / matte**
- **Granulado extra**
- **Vinheta / escurecer bordas**

### Fluxo sugerido
1. Entrar em **Lente Retro**
2. Carregar a foto
3. Aplicar uma **receita pronta** como base
4. Refinar exposição, LUT, nitidez, glow e novos controles retro
5. Exportar em **JPG alto**


## Correção — layout Retro/3D e enquadramento

- As caixas informativas da Lente Retro agora seguem a mesma identidade azul da interface 3D.
- Os painéis recolhíveis foram compactados para evitar proporção grande/desproporcional.
- A estrutura visual foi aproximada novamente da versão anterior do site 3D.
- O preview agora acompanha a rolagem no desktop.
- No modo Retro, o usuário pode mover a imagem arrastando diretamente no preview.
- No modo Retro, o usuário pode dar zoom ou tirar zoom usando o scroll do mouse no preview.
- O reset de enquadramento permanece disponível também na Lente Retro.


## Repaginação visual dos modos

Foi aplicada uma repaginação geral para acomodar melhor os modos Lente 3D e Lente Retro:

- Nova barra superior para alternar entre Lente 3D e Lente Retro.
- Painel lateral redesenhado com cabeçalho e rolagem interna.
- Painéis recolhíveis compactos e mais consistentes.
- Preview fixo no desktop para acompanhar a rolagem.
- Modo Retro com layout mais limpo, sem coluna de vídeo lateral.
- Receitas da Lente Retro organizadas em cards menores.
- Estrutura visual aproximada da versão 3D original, mas preparada para os dois modos.


## Refinamento visual dos painéis laterais

Os painéis recolhíveis da lateral foram refinados para ficar visualmente mais próximos da referência:
- cards maiores e mais limpos;
- badge numérico circular em destaque;
- título e descrição visíveis mesmo recolhidos;
- chevron discreto à direita;
- visual mais elegante e coerente com o restante da interface.


## Correção — receitas Retro clicáveis

- Corrigida a ação dos botões de receitas prontas da Lente Retro.
- Agora o clique é capturado por delegação global, evitando falhas quando o painel tem rolagem interna ou quando o layout muda.
- As receitas aplicam os valores nos controles e forçam atualização do preview quando há imagem carregada.
- Se não houver imagem carregada, a receita fica selecionada e será usada como base ao carregar a foto.


## Correção definitiva — controles Retro

- Corrigido o ajuste manual após selecionar uma receita.
- Temperatura, matte, granulado e vinheta agora têm listeners próprios.
- O preview é redesenhado diretamente no canvas sem depender do controle RGB.
- As receitas continuam funcionando e podem ser refinadas manualmente.
