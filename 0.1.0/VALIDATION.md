# GBWiz 0.1.0 検証記録

2026-10-31（日本時間）。Windows x64版と、GBWiz専用鍵で署名したAndroid release APKを収録しました。旧候補rc1〜rc4は保持しています。

## 今回完了した確認

- Windows全73テスト成功。作成ボーナス、DQ3を含む戦闘報酬、全呪文、名前表示、善悪混合、マップ、保存・倍速などを含みます。
- 配布先Windows EXEで外伝I〜III・GBC版I〜III・DQ3の7作品の180フレーム・映像変化・ステート復元を確認。ユーザー保存先への書込みはありません。
- Windowsの埋込版番号0.1.0、数値0.1.0.0、prereleaseフラグなし。
- Android release・debug・テストAPKとrelease lintVitalのビルド成功。
- 配布APKはapplicationId=jp.gbwiz、versionCode=6、versionName=0.1.0、非debuggable、minSdk=26、targetSdk=35、arm64-v8a／x86_64。
- 専用RSA 3072ビット鍵のAPK署名、v2／v3署名検証、16KBネイティブライブラリ整列の確認。
- 秘密鍵をAGENTS.md指定のGBWiz_signingへ保存。フォルダは所有ユーザーとSYSTEMに限定し、資格情報はWindows DPAPIで暗号化。配布物には含めません。
- Windows ZIPの実行ファイル・DLL・空のRomフォルダ・ライセンスと、署名APKの内容・除外対象・SHA256SUMSを検査。

## 直近の開発版で確認した実機範囲

Pixel 9aのJNI経由で、GBC版3作品の作成ボーナス75条件、外伝IIIの作成100条件、外伝I・IIの作成50条件、DQ3報酬105条件が成功しています。各機能の解析資料には検証の詳細と範囲を記載しています。

## 今回の実機確認と残る範囲

最終作成中に端末が未接続となったため、今回署名した正式APKの実機起動・更新は未確認です。署名が異なる旧開発版を自動削除せず、別IDの検証用releaseビルドまで行っています。検証用APKは配布物には含めません。

既存開発版とは署名が違うため、正式APKでそのまま上書き更新できません。移行はREADME.mdの手順を参照してください。全イベント・全進行段階・長時間プレイ、実物コントローラー、Windows開発環境外での網羅確認は未実施です。Androidの現状の初期ROMフォルダはDocuments/GBWiz/romで、指定のDocuments/NesDQとの整合は残っています。

ソースは別途配布します。公開・アップロード操作は行っていません。
