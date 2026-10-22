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

## GitHub

公式ドキュメント(docs.github.com)のページを直接開いて読むことができなかったため、全行を `未確認` とした。値は素案の値で、Web 検索の要約(公式ページそのものではない)とは矛盾しなかったが、公式ページの記述で確かめるまでは `確認済み` にしない。規約(Terms of Service、Acceptable Use Policies、プライバシーの声明)は読めておらず、抜粋の長さ・帰属表示・保存・再配布の定めは `unverified` とした。確認日と URL は、読んだページがないため `-` とし、確かめる候補のページは値の欄に書いた。

| 項目 | 値 | 状態 | 確認日 | URL |
|---|---|---|---|---|
| endpoint | ベースは https://api.github.com 。素案: GET /search/repositories、GET /search/issues、GET /repos/{owner}/{repo}(確かめる候補: https://docs.github.com/en/rest/search/search 、https://docs.github.com/en/rest/repos/repos 、https://docs.github.com/en/rest/issues/issues) | 未確認 | - | - |
| search_result_cap | 1000(素案: 検索ごとに最大 1,000 件。確かめる候補: https://docs.github.com/en/rest/search/search) | 未確認 | - | - |
| search_rate_limit_authenticated | 30 回/分(素案。確かめる候補: https://docs.github.com/en/rest/search/search の Rate limit の節) | 未確認 | - | - |
| search_rate_limit_unauthenticated | 10 回/分(素案。確かめる候補: https://docs.github.com/en/rest/search/search の Rate limit の節) | 未確認 | - | - |
| core_rate_limit | 素案: 認証なし 60 回/時、認証あり 5,000 回/時。secondary rate limit もある(確かめる候補: https://docs.github.com/en/rest/using-the-rest-api/rate-limits-for-the-rest-api) | 未確認 | - | - |
| api_version | 2022-11-28(素案。設定の既定値。ほかの版が公開されているかは未確認。確かめる候補: https://docs.github.com/en/rest/about-the-rest-api/api-versions) | 未確認 | - | - |
| terms | unverified(GitHub Terms of Service の API の条項と Acceptable Use Policies を読めていない。確かめる候補: https://docs.github.com/en/site-policy/github-terms/github-terms-of-service) | 未確認 | - | - |
| excerpt_max_chars | 500(素案。規約に抜粋の長さの定めがあるか読めていない。詳細設計の仮の値) | 未確認 | - | - |
| rights.license | unverified(User-Generated Content の節とリポジトリごとのライセンスの扱いを読めていない) | 未確認 | - | - |
| rights.attribution_required | unverified(帰属表示の要否を読めていない) | 未確認 | - | - |
| rights.retention_policy | unverified(保存してよい範囲を読めていない。確かめる候補: https://docs.github.com/en/site-policy/acceptable-use-policies/github-acceptable-use-policies) | 未確認 | - | - |
| rights.redistribution_policy | unverified(再配布の可否を読めていない) | 未確認 | - | - |
| rights.eligible_use | unverified(利用目的の制限を読めていない。Acceptable Use Policies の情報の利用の節を確かめる) | 未確認 | - | - |
| rights.documentation_url | unverified(根拠にした公式ページがまだない) | 未確認 | - | - |
| rights.last_reviewed_at | unverified(公式ページを読めていないため審査日を記録しない) | 未確認 | - | - |
