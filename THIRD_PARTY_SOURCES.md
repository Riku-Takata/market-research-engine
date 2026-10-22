# Third-party sources

外部のデータソースについて、公式のドキュメントと規約で確かめた値と、その状態を記録する。
状態が `未確認` の値は、公式の記述で確かめられていない。

## Hacker News

公式 API ドキュメント(HackerNews/API の README)で確かめた値だけを `確認済み` にした。API 専用の利用規約や、抜粋の長さ・帰属表示・保存・再配布の定めは、読んだ範囲では見つからなかったため `未確認` とし、素案の値か `unverified` を置いている。

| 項目 | 値 | 状態 | 確認日 | URL |
|---|---|---|---|---|
| endpoint | ベースは https://hacker-news.firebaseio.com/v0/ 。topstories.json、newstories.json、beststories.json、askstories.json、showstories.json、jobstories.json、item/<id>.json | 確認済み | 2026-10-22 | https://github.com/HackerNews/API |
| list_size | top/new/best は最大 500 件、ask/show/job は最大 200 件 | 確認済み | 2026-10-22 | https://github.com/HackerNews/API |
| rate_limit | 「There is currently no rate limit.」と書かれている(現時点で制限なし) | 確認済み | 2026-10-22 | https://github.com/HackerNews/API |
| terms | unverified(API 専用の利用規約は README に見当たらない。読んだ箇所: HackerNews/API の README。Y Combinator の一般的な法務ページとの関係は未確認) | 未確認 | 2026-10-22 | https://github.com/HackerNews/API |
| excerpt_max_chars | 500(素案。規約に抜粋の長さの定めは見当たらない。読んだ箇所: HackerNews/API の README) | 未確認 | 2026-10-22 | https://github.com/HackerNews/API |
| rights.license | unverified(API のデータのライセンスの明記は見当たらない) | 未確認 | 2026-10-22 | https://github.com/HackerNews/API |
| rights.attribution_required | unverified(帰属表示を求める明確な記述は見当たらない) | 未確認 | 2026-10-22 | https://github.com/HackerNews/API |
| rights.retention_policy | unverified(保存の可否・期間の明確な記述は見当たらない) | 未確認 | 2026-10-22 | https://github.com/HackerNews/API |
| rights.redistribution_policy | unverified(再配布の可否の明確な記述は見当たらない) | 未確認 | 2026-10-22 | https://github.com/HackerNews/API |
| rights.eligible_use | unverified(利用目的の制限の明確な記述は見当たらない) | 未確認 | 2026-10-22 | https://github.com/HackerNews/API |
| rights.documentation_url | https://github.com/HackerNews/API | 確認済み | 2026-10-22 | https://github.com/HackerNews/API |
| rights.last_reviewed_at | 2026-10-22 | 確認済み | 2026-10-22 | https://github.com/HackerNews/API |
