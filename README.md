# lw-frontend-dist

Longevity Watch の OTA バンドルの配信先です。**中身は CI が書きます。**
手で置かないでください。

- `dist/<版>/<版>.zip` … バンドル本体
- `dist/<版>/<版>.zip.sig` … Ed25519 の署名
- `dist/version_info-<x.y>.json` … いまどの版を配っているか

アプリは署名を検証してから適用します。検証できないものは適用しません。
