# Painel administrativo

Esta pasta publica o painel em `/admin` junto do site principal. Ele conversa
somente com o Worker em `api.nostalgiaservicos.site`; o computador não fica
aberto para a internet.

Antes de publicar, configure no Worker o secret `NOSTALGIA_ADMIN_PASSWORD`
com uma senha forte escolhida por você. Em seguida, publique o Worker a partir
da pasta principal do Nostalgia. O painel usa o banco D1 já existente, portanto
não exige outro banco de dados.

O programa no computador busca os comandos do painel automaticamente. Por
enquanto o painel permite acompanhar pedidos e conversas e pausar, retomar ou
forçar a sincronização da fila. Novos controles podem ser adicionados sem
alterar a página pública do site.
