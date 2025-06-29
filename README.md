# sepic-svr-maintenance
Sepic鯖のメンテナンス計画と変更ログ置き場


> メンテナンスにあたって
 - 使い方が分からないAppは[HowToUseApp](/HowToUseAPP/README.md)を閲覧してください。
- 使い方が分からないMinecraft Pluginは[mc-plugins](/mc-plugins/README.md)を閲覧してください。
 - 変更にvelocityやminecraftを落とす必要がある際は、事前に最低でも@hereで連絡すること。
 - 変更にvelocityやminecraftを落とす必要がない場合は、簡易的な(メンションなし可)連絡をすること。
 - [`ScheduledChanges`](ScheduledChanges)にある変更内容が書かれたファイルは、その内容になるように変更したのち、[`ChangedLogs`](ChangedLogs)に移動をすること。
 - [`ScheduledChanges`](ScheduledChanges)や[`ChangedLogs`](ChangedLogs)に追加・入れ替えをした際は、その都度、コミットのコメント欄にそのファイル名と作業内容を記すこと。
    - 例：　コミットコメント-> `250624_1 | EnderPlusをEnderVaultに変更 `

<br>
<br>

> *ScheduledChanges*や*ChangedLogs*のファイル命名
- ファイル命名は次の通りである。
    - yymmdd_no.md
    - yymmddの日付は、変更実施予定日を記すこと。<br>　※変更予定日を過ぎた場合でも、ファイル名の変更はしないこと。
    - `_no`のnoはその日の変更の何個目かを記すこと。<br>　※変更数が1つの場合でも、1とする。
        - 例: 2025年6月24日実施の変更1つ目 **-->** `250624_1.md`


<br><br><br>

※不備や追加情報があればお知らせください。
readmeの変更日時 | day 2025.06.28 | time 1838/24