# Informativo do Cooperado — Unimed Uberlândia

Publicação semanal do informativo, servida por GitHub Pages e embedada no site do Framer.

## Como funciona

- `index.html` é o informativo completo: layout, estilos e conteúdo num arquivo só.
- O arquivo é **gerado e enviado automaticamente** pelo Montador de Informativo. Não edite à mão.
- Publicar no montador substitui este arquivo e o site atualiza em cerca de um minuto.

## Endereços

| Uso | Endereço |
| --- | --- |
| Home | `https://informativoudi.github.io/informativounimeduberlandia/` |
| Espelho | `https://informativoudi.github.io/informativounimeduberlandia/?espelho=true` |

No Framer, cada endereço vai num bloco de Embed — a home na página principal, o espelho na `/espelho`.

## Fluxo semanal

1. A analista mantém o Word das pautas online.
2. O montador importa o Word e monta a edição com status **Espelho**.
3. Validação na página `/espelho`.
4. Botão **Publicar no site**: a edição vira a atual, a anterior vai para o histórico e o commit sobe sozinho.

## Configuração do Pages

Settings → Pages → Source: *Deploy from a branch* → branch `main`, pasta `/ (root)`.
