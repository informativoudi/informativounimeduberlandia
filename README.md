# Informativo do Cooperado — Unimed Uberlândia

Publicação semanal do informativo, servida por GitHub Pages e embedada no site do Framer.

## Como funciona

- `index.html` é o informativo completo: cabeçalho, layout, estilos e conteúdo num arquivo só.
- O arquivo é **gerado e enviado automaticamente** pelo Montador. Não edite à mão.
- `montador.html` é a ferramenta de montagem. Aberta aqui pelo GitHub Pages, pede usuário e senha da equipe.
  Aberta no computador (arquivo baixado), entra em **modo de teste**: dá para editar e ver a prévia, mas nada é publicado.
- `acesso.json` guarda a equipe (usuários) de forma criptografada.

## Ramos (branches)

| Ramo | O que guarda | Atualiza o site? |
| --- | --- | --- |
| `main` | `index.html`, `montador.html`, `acesso.json` | **Sim** — o GitHub Pages publica este ramo |
| `rascunhos` | `dados.json` (rascunhos da equipe, salvos a cada alteração) | Não |

O ramo `rascunhos` é criado sozinho pelo montador na primeira vez que alguém salva, e o rascunho antigo
que estava no `main` é copiado para ele automaticamente. Assim, salvar rascunho não dispara mais
atualização do site: só **Publicar no site** e **Enviar ao espelho** atualizam o GitHub Pages.

Depois que o montador novo estiver em uso, o `dados.json` que ficou no `main` não é mais usado e pode ser apagado.

## Endereços

| Uso | Endereço |
| --- | --- |
| Home | `https://informativoudi.github.io/informativounimeduberlandia/` |
| Espelho | `https://informativoudi.github.io/informativounimeduberlandia/?espelho=true` |
| Montador | `https://informativoudi.github.io/informativounimeduberlandia/montador.html` |

## Fluxo semanal

1. A analista mantém o Word das pautas online.
2. O montador importa o Word e monta a edição com status **Espelho**.
3. Validação na página `/espelho` (botão **Enviar ao espelho**).
4. Botão **Publicar no site**: a edição vira a atual, a anterior vai para o histórico e o commit sobe sozinho.

## Configuração do Pages

Settings → Pages → Source: *Deploy from a branch* → branch `main`, pasta `/ (root)`.
