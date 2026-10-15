# 友達招待ページ (GitHub Pages)

`InviteLink`(アプリ側)が作る `https://nanashinogonn.github.io/i/?t=<トークン>` の受け皿。

- `i/index.html`: 招待ページ。「アプリで開く」(`scrapp://invite/<トークン>`)と「App Storeで入手」
- `.well-known/apple-app-site-association`: ユニバーサルリンク用。`/i/*` をアプリで開く
- `.nojekyll`: これが無いと `.well-known` フォルダが公開されない

このフォルダの中身を、GitHubの `nanashinogonn.github.io` リポジトリの直下にそのまま置く
(ユーザーサイトのリポジトリでないと、ドメイン直下の `.well-known` に置けない)。
`i/index.html` の `APP_STORE_ID` は App Store Connect のアプリの Apple ID(6800409811)。
