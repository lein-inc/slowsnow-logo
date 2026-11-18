# slow snow STUDIO — ロゴ提案サイト

staticrypt でパスワード暗号化した静的ページ。PDF・音源は暗号化 HTML 内に埋め込み（平文ファイルは置かない）。

再ビルド: `src/*.html` を編集 → `npx staticrypt src/<name>.html -p '<password>' --short --remember 30 -d .` → テンプレートは docs_src/password_template_mono.html（モノクロ）。日本語文言は --template-* オプションで指定（CHANGELOG 参照）。

## 2026-11-18 決定版ページ
- `final.html`（src/final.html）: B-1 SSS＋Jost の納品データページ。ガイド 3p スライド＋ Google Drive リンク（ZIP 27MB・ガイド PDF）。生成元は `~/Desktop/claude_data/slowsnow_logo/final/build_site_page.py`。
- 再暗号化コマンド（index/final。salt は .staticrypt.json を共有）:
  `STATICRYPT_PASSWORD="slowsnow-2026" npx -y staticrypt src/index.html src/final.html -d . --short --remember 30 -t docs_src/password_template_mono.html --template-title "slow snow STUDIO — ロゴ提案" --template-instructions "パスワードを入力してください" --template-button "閲覧する" --template-placeholder "パスワード" --template-error "パスワードが違います" --template-toggle-show "パスワード表示" --template-toggle-hide "パスワード非表示"`
