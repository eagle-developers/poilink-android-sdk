# Poilink SDK for Android

Android 向け Poilink SDK。ユーザ認証、WebPortal 表示、ミッション進捗管理、アカウント引き継ぎ機能を提供します。

ドキュメント: [https://docs.poilink.com/android/](https://docs.poilink.com/android/)

---

## 動作要件

| 項目 | バージョン |
|---|---|
| Android Min SDK | API 26 (Android 8.0) 以上 |
| Android Target SDK | 34 以上 (Google Play 公開要件に準拠) |
| Android Compile SDK | 33 以上 |
| Java | 8 (1.8) 以上 |
| 対応 ABI | arm64-v8a / armeabi-v7a / x86_64 |

---

## インストール

### 1. リポジトリを追加する

プロジェクトの `settings.gradle` に Maven リポジトリを追加します。

```groovy
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()
        maven { url 'https://raw.githubusercontent.com/eagle-developers/poilink-android-sdk/1.0.0/maven' }
    }
}
```

### 2. 依存を追加する

アプリモジュールの `build.gradle` に依存を追加します。

```groovy
dependencies {
    implementation 'com.poilink:sdk:1.0.0'
}
```

`play-services-ads-identifier` は SDK の POM に宣言済みのため、個別に追加する必要はありません。

詳細なセットアップ手順 (CLIENT_ID / CLIENT_SECRET の設定、パーミッション、ProGuard / R8、ネットワーク要件等) は [ドキュメントサイト](https://docs.poilink.com/android/) を参照してください。

---

## ライセンス

[LICENSE.md](LICENSE.md) を参照してください。
