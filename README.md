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


## Accordion exclusivo dos painéis

- Agora, ao abrir um painel, os outros painéis recolhem automaticamente.
- Isso evita que as opções desçam demais e fiquem inacessíveis.
- A rolagem interna continua funcionando dentro do painel aberto.
- Os balões azuis dos painéis foram trocados por símbolos legíveis:
  - ↥ Importar / alinhar
  - ✦ Estilo / acabamento
  - ↧ Exportar


## Ajustes desta versão

- Corrigido o visual dos balões azuis dos painéis com ícones limpos e centralizados.
- Ao alternar entre **Lente 3D** e **Lente Retro**, todos os **ajustes criativos** são zerados automaticamente:
  - filtro vintage / LUT
  - intensidade
  - exposição
  - nitidez
  - glow
  - temperatura / warmth
  - fade
  - granulado
  - vinheta
  - RGB displacement
  - interpolação de quadros
  - marca d'água


## Ícones SVG definitivos dos painéis

- Os balões dos painéis agora usam SVG inline, evitando falhas de renderização de símbolos Unicode.
- Ícones:
  - Upload / importar
  - Brilho / ajustes criativos
  - Download / exportar


## Ícones externos em assets/icons

Os ícones dos painéis agora são arquivos SVG externos, referenciados diretamente no HTML.

Pasta criada:

```text
assets/icons/
├── icon-upload.svg
├── icon-sparkle.svg
└── icon-download.svg
```

Referências usadas no sistema:

```html
<img class="tool-group-icon" src="assets/icons/icon-upload.svg" alt="Importar">
<img class="tool-group-icon" src="assets/icons/icon-sparkle.svg" alt="Ajustes">
<img class="tool-group-icon" src="assets/icons/icon-download.svg" alt="Exportar">
```

Isso evita falhas de renderização de símbolos Unicode ou pseudo-elementos CSS.


## Modo de segurança na exportação

Foi adicionada uma camada de compatibilidade para casos em que o usuário exporta vídeo e o arquivo sai preto.

### O que mudou

- Novo switch no painel **Exportar arquivo**: **Modo de segurança na exportação**.
- Aviso amigável quando o modo compatível estiver ativo.
- Detecção preventiva de ambientes com maior risco, como Safari, iOS e mobile.
- Validação básica dos frames antes da exportação.
- Redesenho dos frames antes de exportar, se o sistema detectar risco de frame preto.
- Redução automática de resolução para até 1280px de largura no modo compatível.
- Uso de canvas sem alpha e fundo sólido para reduzir risco de frames pretos.
- Fallback de codec para WebM quando o navegador não lidar bem com MP4/MOV.

### Orientação para usuário

Se o vídeo exportado sair preto:
1. Ative o modo de segurança.
2. Exporte novamente.
3. Se ainda falhar, tente GIF ou JPG alto.
4. Em Safari/iPhone, testar também no Chrome ou em desktop.


## Correção do preview após modo de segurança

- Corrigido problema em que a imagem carregada ficava preta no preview.
- A validação do modo de segurança agora roda somente na exportação, não no preview.
- O preview voltou a usar a renderização normal da ferramenta.
- O modo compatível continua disponível apenas para evitar arquivo preto ao exportar vídeo.


## Botão de exportação abaixo do fluxo

- Adicionado um botão extra de exportação abaixo do card **Fluxo de produção**.
- O botão chama a mesma função de exportação do painel principal.
- O texto muda conforme o modo:
  - Lente 3D: gerar GIF/MP4/MOV conforme formato escolhido.
  - Lente Retro: exportar JPG alto.
- Quando o arquivo fica pronto, o link de download também aparece abaixo do fluxo.


## Correção do botão de exportar abaixo do fluxo

- Corrigido o botão extra de exportação que ficava apagado/desativado.
- Agora ele ativa quando existem frames prontos para exportar.
- O botão não depende mais apenas do estado visual do botão principal.
- O texto continua sincronizado com o formato escolhido.


## Correção visual final dos selos de painel recolhível

- Removido definitivamente o visual de ícone/bolinha dos painéis.
- O antigo balão agora virou um selo textual horizontal: **Painel recolhível**.
- O selo fica pulsando de forma discreta.
- A indicação de rolagem foi mantida como texto auxiliar: **opções abaixo**.


## Remoção definitiva dos balões/ícones antigos

- Os antigos círculos/balões das categorias foram ocultados completamente.
- O aviso **PAINEL RECOLHÍVEL** agora aparece como selo textual no topo do card, fora da área do antigo ícone.
- A indicação **opções abaixo** continua aparecendo como apoio visual para rolagem.


## Vinheta, grão e Dust and Scratches na Lente 3D

- Adicionados controles criativos na guia **Ajustes e Exportar** da Lente 3D:
  - Vinheta / escurecer bordas
  - Granulado extra
  - Dust and Scratches / poeira de filme
- Os efeitos aparecem no preview e entram no arquivo exportado.
- Os controles também são zerados ao alternar entre Lente 3D e Lente Retro.


## Correção de visibilidade dos efeitos criativos na Lente 3D

- Corrigido o painel **Ajustes e Exportar** para exibir os novos controles na Lente 3D:
  - Grão criativo
  - Vinheta criativa
  - Dust and Scratches
- Os controles agora aparecem junto dos demais ajustes criativos, antes de RGB/interpolação/exportação.


## Correção dos efeitos criativos da Lente 3D

- Removidos da Lente 3D os controles que pertencem à Lente Retro:
  - Temperatura / tom quente-frio
  - Pretos desbotados / matte
- Mantidos na Lente 3D:
  - Grão criativo
  - Vinheta criativa
  - Dust and Scratches
- Corrigido o preview ao vivo: grão, vinheta e Dust and Scratches atualizam imediatamente ao mexer na barra.


## Interpolação inteligente controlada pela barra

- A interpolação foi melhorada sem adicionar novos controles.
- Continua sendo controlada pela barra existente de interpolação.
- Não foi aplicado crop automático.
- Não foi aplicada equalização automática.
- Não foi aplicada microvariação analógica.
- O sistema agora usa uma curva mais suave entre os frames e evita interpolar a volta brusca quando o loop não está em ida-e-volta.
- A quantidade de frames intermediários é definida automaticamente pela porcentagem da barra.


## Botão de compra da Lente Retro

- Removido o texto **Feito In 3D • ferramenta experimental** do site.
- Atualizado o texto do botão da Lente 3D para **Comprar Lente 3D**.
- Adicionado botão **Comprar Lente Retro** ao lado do botão da Lente 3D.
- Link da Lente Retro: https://www.mercadolivre.com.br/lente-retro-30mm-feitoin3d-canon-sony-nikon-fuji/up/MLBU3825743208#polycard_client=search-desktop&be_origin=backend&search_layout=grid&position=1&type=product&tracking_id=6a1e9caa-25cc-47cc-ade7-fb764a2a25c4&wid=MLB4502712035&sid=search


## Botão Retro branco e ajuste fino mais responsivo

- O botão **Comprar Lente Retro** agora usa visual branco, igual ao botão da Lente 3D.
- O ajuste fino por frame ficou mais responsivo:
  - clique normal nas setas move 4px;
  - Shift + clique move 1px para ajuste super fino.
- A atualização do ajuste fino ficou mais leve, evitando redesenhar miniaturas a cada clique.


## Ajuste fino com navegação de frames e play/pause

- Restaurada a navegação entre frames dentro do painel de ajuste fino.
- Adicionado botão para pausar/reproduzir o preview do GIF.
- Ao entrar no ajuste fino, o preview pausa para edição, mas o usuário pode retomar a reprodução.
- O ajuste rápido por setas permanece:
  - clique normal move 4px;
  - Shift + clique move 1px.


## Ajuste fino com design limpo restaurado

- Esta versão volta a partir da versão anterior ao experimento Preview Editor.
- O painel de ajuste fino volta ao design limpo:
  - título;
  - botão Minimizar;
  - botão compacto Reproduzir/Pausar no cabeçalho;
  - navegação Preview / Frame 1 / Frame 2 / Frame 3;
  - setas de ajuste.
- Os botões grandes de pausa/reprodução foram removidos.
- As funções recentes foram mantidas:
  - clique normal move 4px;
  - Shift + clique move 1px;
  - é possível pausar e retomar a reprodução do GIF.


## Ajuste fino minimizado por padrão

- O painel de ajuste fino agora abre minimizado.
- Enquanto minimizado, aparece apenas o cabeçalho e o botão **Mostrar**.
- As ferramentas internas só aparecem quando o usuário clicar em **Mostrar**.
- As funções anteriores foram mantidas:
  - navegação Preview / Frame 1 / Frame 2 / Frame 3;
  - botão Reproduzir/Pausar;
  - clique normal move 4px;
  - Shift + clique move 1px.


## Correção final do painel de ajuste fino limpo

- Removido o botão extra **Reproduzir** do cabeçalho.
- O botão **Minimizar** voltou a aparecer no cabeçalho do painel expandido.
- O botão **Preview** da navegação agora se chama **Reproduzir**.
- O visual das setas foi corrigido para voltar ao formato quadrado/limpo.
- O painel continua minimizado por padrão e só mostra as ferramentas ao clicar em **Mostrar**.


## Correção de overflow do painel de ajuste fino

- O painel de ajuste fino foi limitado à largura do preview.
- O painel não deve mais vazar para fora da tela.
- O botão **Minimizar** permanece visível quando o painel está aberto.
- Quando minimizado, aparece apenas o cabeçalho com **Mostrar**.
- A navegação Reproduzir / Frame 1 / Frame 2 / Frame 3 e as setas foram mantidas.
