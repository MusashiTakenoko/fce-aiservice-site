# fce-aiservice.com 公開用ファイル一式

## 概要

- 完全な静的サイトです（HTML / CSS / JS のみ）。**ビルド作業・サーバーサイド処理・DBは一切不要**です。
- このフォルダの中身を、そのまま **fce-aiservice.com のドキュメントルート直下**に配置すれば動作します。

## お願いしたいこと

1. **本フォルダ一式の配置・公開**（fce-aiservice.com のドキュメントルート直下にそのまま配置）
2. **SSL（HTTPS）の有効化**（各ページのcanonical URLがhttpsのため必須）

## サイト構成

| URL                          | ファイル                        | 内容                              |
|------------------------------|---------------------------------|-----------------------------------|
| /                            | index.html                      | 親サイト（FCEのAIソリューション） |
| /aitraining/                 | aitraining/index.html           | FCEのAI研修                       |
| /aitraining/contact/         | aitraining/contact/index.html   | 資料請求・お問い合わせ            |
| /elearning/                  | elearning/index.html            | eラーニング講座                   |

- ルート直下のその他のファイルは画像アセット（png / svg）、robots.txt、sitemap.xml です。
- 各ディレクトリ（/aitraining/ /elearning/ など）へのアクセス時に `index.html` が返る設定（一般的なWebサーバーのデフォルト）を前提としています。

## 技術メモ

- 外部通信: Google Fonts（fonts.googleapis.com / fonts.gstatic.com）と、お問い合わせフォームのkintone埋め込みiframe（*.form.kintoneapp.com）のみ。
- `.svg` ファイルが `image/svg+xml` のMIMEタイプで配信されることをご確認ください（通常はデフォルトで問題ありません）。
- canonical / OGP / sitemap.xml / robots.txt はすべて https://fce-aiservice.com/ 基準で設定済みです。URL構成を変える場合はご相談ください。
- 将来 fce-aiservice.com 直下に別コンテンツ（総合サイトの拡張など）を追加する場合も、本構成とは競合しません。

## 連絡先

内容・修正のご相談: 河野（マーケティング）
