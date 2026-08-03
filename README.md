# qiita-images

Qiita 記事から raw URL で参照する画像置き場（public）。

- 追加は iobsidian の `.claude/skills/platform-qiita/scripts/upload_qiita_images.py` 経由で行う
- **同名上書き禁止**。スクリプトが内容ハッシュをファイル名に付けるので、差し替えは常に新ファイル + 記事側の URL 貼り替えで行う（raw と Qiita プロキシの二重キャッシュがあり、上書きしても反映されないため）
- public リポジトリなので、機密情報が写り込んだ画像は絶対に置かない（push したら事実上消せない）
