# GBWiz 0.1.0-rc2 リリース候補

## Windows

Windowsフォルダ内のGBWiz.exeを起動し、GB／GBCのROMを選択してください。初期位置は同じフォルダのRomです。ROMは含みません。
通常セーブ・設定・ステートは`%APPDATA%\GBWiz`へROM名に基づいて保存します。

矢印で移動、X=A、Z=B、Enter=Start、右Shift=Select、F1／Esc=機能メニュー、F5=スロット1保存、F8=読込。
倍率・速度・ON／OFFはメニューの左右で変更します。Xbox／Proでは左スティック押し込み=メニュー、LT=保存、右スティック押し込み=読込です。

## Android

Android 8.0以降、arm64-v8a／x86_64向けです。候補に含む`unsigned.apk`は正式署名前の成果物で、そのままインストールする配布版ではありません。
正式署名は、プロジェクトの`sign-release.ps1`とGBWiz専用鍵で行います。署名鍵・パスワードは配布物に含めません。
既存の開発版と正式署名版は署名が異なるため、そのまま上書き更新できません。正式版への切替手順は署名確定後に案内します。

現在のAndroid初期ROMフォルダはDocuments/GBWiz/romで、任意フォルダへ変更できます。AGENTS.md指定のDocuments/NesDQとの整合は残件です。
設定・通常セーブ・ステートは選択したDocuments/GBWiz配下に保存します。

## 収録物

- Windows実行ファイル・SDL2.dll、空のRomフォルダ、操作説明。
- Android未署名release APK（Android成果物を含めて作成した場合）。
- この候補に対応するソースZIP、GPL・SDL2・blipperのライセンス、リリースノート、SHA256SUMS。

ソースZIPはAndroidのGradle wrapper・Java／JNI・リソース、WindowsのCMake・RC・ICO、依存コードを含みます。ROM、通常セーブ、ステート、秘密鍵、ローカルSDK設定、ビルドキャッシュは含みません。
SHA256SUMSは配布物の確認用であり、ROMの判別・セーブ名には使用しません。
