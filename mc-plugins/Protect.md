# Protect Plugin<sup><span style="color: red; ">_これはまだ下書き段階のドキュメントです!!_</span></sup>

これは建築保護(WorldGuardの軽量代替)プラグインです。\
GithubやModrinthでは詳しく説明されていないので、日本語訳として残しておきます。\
エリア選択はWEかFAWEの`//pos1 x,x,x`や`//pos2 x,x,x`で選択しないといけないところは注意ポイントです。\
[コマンド](#コマンド)でコマンドについて記述していますが、詳しくは後述します。
<br>

> 見出し
- a
- b
    - ba

<br><br><br>

## コマンド
| command  |    説明  |permission|
|----------|----------|----------|
|`/area create <name> [<priority>]`|新しい保護エリアを作る|protect.command.area.create|
|`/area delete <area>`|既存の保護エリアを削除する|protect.command.area.delete|
|`/area flag info [flag] (area)`|エリアフラグに関する情報を照会する|protect.command.area.flag.info|
|`/area flag list [<provider>]`|指定されたエリアのフラグすべてをリスト表示する|protect.command.area.flag.list|
|`/area flag reset <flag> [<area>]`|指定されたエリアのフラグをリセットする|protect.command.area.flag.reset|
|`/area flag set <flag> <value> [<area>]`|指定されたエリアのフラグを変更する|protect.command.area.flag.set|
|`/area group add <group> [<name>]`|現在の選択をグループに追加(?)<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.group.add|
|`/area group create <area>`|入力されたエリアからグループを作成する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.group.create|
|`/area group delete <group>`|グループの削除(グループ内のエリア事態は削除されません)<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.group.delete|
|`/area group list [<group>]`|すべてのグループまたは、グループの領域をリストで表示します<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.group.list|
|`/area group redefine <group> <region>`|グループ内の領域を再定義する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.group.redefine|
|`/area group remove <group> <region>`|グループからエリアを削除する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.group.remove|
|`/area group select <group> <region>`|グループ内の領域を選択する<sup><span style="color: red; ">_検証待ち_</span></sup>|worldedit.selection.pos|
|`/area info [<area>]`|特定のエリアに関する情報を見る|protect.command.area.info|
|`/area list`|現在あるエリア全てをリストで表示します|protect.command.area.list|
|`/area members add <area> <players>`|エリアメンバーを追加する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.members.add|
|`/area members list [<area>]`|エリアメンバーを一覧表示する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.members.list|
|`/area members remove <player>`|エリアメンバーを削除する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.members.remove|
|`/area owner remove <player>`|エリアの所有者を削除する|protect.command.area.owner.remove|
|`/area owner set <area> <player>`|エリアの所有者を設定する|protect.command.area.owner.set|
|`/area parent remove <area>`|エリアの親を削除する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.parent.remove|
|`/area parent set <area> <parent>`|エリアの親を設定する(ツリーかな？)<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.parent.set|
|`/area priority <area> [<priority>]`|エリアの優先順位を表示または削除する<sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.priority|
|`/area protect <area> [remove]`|エリアの保護を追加・更新または削除をします|protect.command.area.protect|
|`/area redefine <area>`|既存のエリアの領域を再定義する|protect.command.area.redefine|
|`/area schematic delete <area>`|エリアのschematicを削除する <sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.schematic.delete|
|`/area schematic load <area>`|エリアのschematicを読み込む <sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.schematic.load|
|`/area schematic save <area>`|エリアのschematicを保存する <sup><span style="color: red; ">_検証待ち_</span></sup>|protect.command.area.schematic.save|
|`/area select <area>`|既存エリアの領域を選択する<sub>(WorldWdit)</sub><sup><span style="color: red; ">_検証待ち_</span></sup>|worldedit.selection.pos|
|`/area teleport <area>`|任意のエリアへTPする|protect.command.area.teleport|








k
|``|||
|``|||
|``|||