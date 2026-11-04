# slow snow STUDIO — ロゴ提案サイト

staticrypt でパスワード暗号化した静的ページ。PDF・音源は暗号化 HTML 内に埋め込み（平文ファイルは置かない）。

再ビルド: `src/*.html` を編集 → `npx staticrypt src/<name>.html -p '<password>' --short --remember 30 -d .` → テンプレートは docs_src/password_template_mono.html（モノクロ）。日本語文言は --template-* オプションで指定（CHANGELOG 参照）。
