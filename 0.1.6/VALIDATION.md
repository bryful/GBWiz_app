# GBWiz 0.1.6 検証結果

2026-11-21。

- Windows x64 Release、Android Release（arm64-v8a／x86_64）のビルドに成功しました。Android lintReleaseも成功しました（エラー0、警告12）。
- 関連テスト３件（items_gaiden1、items_all_wizardry、item_names_gbc）がすべて成功しました。
- Wizardry全６作品で、アイテムの装備・解除・受け渡し・一括移動と保存整合性を確認しました。並べ替え・削除確認・呪いの除外は共通処理の外伝Iテストでも確認しています。
- GBC３作品では原作操作による酒場・商店の到達と、編集メニューの使用可否も確認しました。
- GBC版の識別済み・未識別名、計1,218件（未使用番号の代替表示を含む）の読み取りが成功しました。Windows実画面で原作フォントの日本語表示を確認しました。
- Androidのパッケージ名jp.gbwiz、versionCode 12、versionName 0.1.6、最低SDK 26、対象SDK 35、両ABIを確認しました。
- Android署名v2／v3、0.1.5との証明書一致、APKおよび両ABIのELFの16KB整列を確認しました。
- Android実機での今回のAPKのインストール・表示・操作は未確認です。
- 全テスト一式や全アイテム・全職業の装備組み合わせは再検証していません。今回の変更に関係する確認に限定しています。
