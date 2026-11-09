# Placar Pife e Uno

Placar de vitórias para dois jogadores. Feito para Paulo e Manu acompanharem quem está ganhando no **Pife** e no **Uno**, e aceita outros jogos de mesa, como Truco, Dominó e Xadrez.

A tela inteira cabe na altura do celular, sem rolar. Só as Estatísticas, o Histórico e o Geral rolam, porque têm muito conteúdo.

O app conta só vitórias, sem pontos e sem limite. A cada partida, quem ganhou toca no botão, e o placar, as médias e o histórico se atualizam na hora. O visual é de giz de cera em cores pastel, inspirado nos jogos de plataforma do Super Nintendo, com movimentos em poucos quadros, como uma animação desenhada à mão.

É um único arquivo (`index.html`), sem servidor e sem instalação de pacotes. Também funciona como app instalável (PWA), inclusive sem internet.

## O que dá para fazer

- **Placar por jogo.** Pife e Uno já vêm prontos, cada um com seu visual (cartas de baralho no Pife, cartas coloridas no Uno).
- **Jogos novos.** Crie até 4 jogos (sugestões: Truco, Dominó, Xadrez, Dama, Buraco), escolhendo nome, símbolos e cores.
- **Estatísticas.** Vitórias, aproveitamento, maior sequência, sequência atual, maior vantagem, últimas 10 partidas e gráfico de vitórias acumuladas.
- **Geral.** Resumo que soma todos os jogos, com o placar de cada um.
- **Período.** Filtro "Tudo", "Este mês" ou "7 dias" que vale para o placar, as estatísticas, o histórico e o resumo geral.
- **Comemoração.** A cada vitória o ovo do jogador pula e solta estrelas, flores e ovinhos. Sequências de 3, 5, 10 (e de 5 em 5 depois) ganham uma faixa de destaque.
- **Loja.** Cada vitória vale 1 de saldo para quem ganhou. Com o saldo, cada jogador compra o que quiser: 5 fundos para o contador (Bolinhas, Gramado, Nuvens, Pôr do sol e Noite estrelada) e 5 animações de vitória (Chuva de ovos, Jardim, Corações, Estrelas cadentes e Fogos de giz), a 10, 20, 30, 40 e 50 vitórias. Toque no desenho de uma animação para ver como ela fica.
- **Compartilhar como imagem.** Gera um cartão com o placar (geral ou de um jogo) para salvar ou enviar pelo celular.
- **Histórico.** Lista de partidas com data e hora, com opção de excluir, e botão para desfazer a última vitória.
- **Modo claro e escuro**, seguindo o aparelho.
- **Backup.** Copie todos os dados como texto e restaure em outro aparelho ou navegador.

## Como usar

1. Abra o `index.html` no navegador (dois cliques no arquivo) ou publique a pasta, como descrito abaixo.
2. Escolha o jogo no topo (Pife, Uno ou um jogo que você criou).
3. Quando alguém ganhar uma partida, toque no botão do jogador.
4. Veja as médias na aba **Estatísticas**, o registro na aba **Histórico** e o resumo dos jogos em **Geral**.
5. Na aba **Loja**, gaste as vitórias em fundos e animações. Cada jogador tem o seu saldo e o seu visual.
6. No ícone de engrenagem, no topo, ficam os **Ajustes e backup**: dá para trocar os nomes (começam como Paulo e Manu), copiar ou restaurar os dados, zerar o placar de um jogo ou excluir um jogo criado por você.

Os dados ficam salvos no próprio navegador do aparelho (`localStorage`). Cada aparelho tem o seu placar. Para levar os dados de um aparelho para outro, use **Copiar dados** em um e **Restaurar** no outro.

## Baixar e instalar no celular

Para usar como app, a pasta precisa estar publicada em um endereço `https`. O jeito mais simples é o GitHub Pages:

1. No repositório, abra **Settings > Pages**.
2. Em **Build and deployment**, escolha **Deploy from a branch**, branch `main` e pasta `/ (root)`.
3. Aguarde um minuto e abra o endereço indicado (`https://SEU-USUARIO.github.io/placar-pife/`).
4. No celular, use **Adicionar à tela inicial** (Chrome e Safari). O app abre em tela cheia, com o ícone do ovo, e continua funcionando sem internet.

Para rodar no computador sem publicar, abra o `index.html` direto no navegador. O modo instalável e o uso sem internet só funcionam quando a pasta é servida por `http` ou `https`.

## Arquivos

| Arquivo | Para que serve |
| --- | --- |
| `index.html` | O app inteiro: página, estilos e código. |
| `manifest.webmanifest` | Nome, cores e ícones do app instalável. |
| `sw.js` | Guarda o app no aparelho para abrir sem internet. Ao mudar o app, aumente `VERSION` no começo do arquivo. |
| `icons/` | Ícones: um ovo manchado com risquinhos de contagem, sobre colinas e céu. |

As fontes (Chewy e Fredoka) vêm do Google Fonts. Sem internet na primeira abertura, o app usa fontes parecidas do sistema.

## Sobre o visual

O estilo é inspirado no visual de giz de cera e aquarela de Yoshi's Island, do Super Nintendo. É um projeto pessoal, sem ligação com a Nintendo. Não usa personagens, imagens, músicas nem logos do jogo: os ovos, colinas, nuvens e flores foram desenhados do zero para este app.
