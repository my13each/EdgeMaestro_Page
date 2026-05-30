---
layout: default
title: Edge Maestro — Privacy Policy
---

# Edge Maestro — Privacy Policy

**Last updated:** 2026-05-30

Languages: [English](#english) · [日本語](#japanese) · [한국어](#korean)

---

## English

### TL;DR

Edge Maestro **does not collect, transmit, or share any data**. Everything stays on your device.

### 1. Information we collect

**None.** Edge Maestro does not collect any personal information, usage data, telemetry, crash reports, or analytics of any kind.

### 2. Information stored on your device

Your gesture mappings, action preferences, and visual settings are stored locally on your device using Android's DataStore. This data:

- Stays only on your device
- Is **not** synchronized, **not** backed up to the cloud (`allowBackup` is disabled), and **not** transmitted anywhere
- Can be cleared at any time by clearing the app's storage from system settings, or by uninstalling the app

### 3. Network usage

Edge Maestro does not use the internet. The app does **not declare the `INTERNET` permission**, which means Android itself prevents the app from making any network connection. This is verifiable from the app manifest.

### 4. Permissions and why they are required

| Permission | Why |
|---|---|
| Display over other apps (`SYSTEM_ALERT_WINDOW`) | To draw the edge gesture overlay on top of other apps. |
| Foreground service (`FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_SPECIAL_USE`) | To keep gesture detection running reliably while the service is active. |
| Accessibility service (`BIND_ACCESSIBILITY_SERVICE`) | To dispatch the actions you've configured (back, home, recents, simulated touches). Edge Maestro does **not** read screen text, capture passwords, or record any user input. The accessibility API is used solely to perform user-initiated actions. Additionally, the service reads only the on-screen position (`bounds.top`) of the soft keyboard (IME) window so that trigger zones can avoid overlapping the keyboard while you type — the text, UI elements, or input contents of the IME window are never accessed. |
| Notifications (`POST_NOTIFICATIONS`) | To display the foreground-service notification required by Android 13 and later. |
| Auto-start at boot (`RECEIVE_BOOT_COMPLETED`) | To resume the gesture service after device reboot when you have enabled it. |
| Query installed apps (`<queries>`) | To list launcher apps so you can choose which app to open from a gesture. The list of apps is read locally and never leaves your device. |

### 5. Third-party services and SDKs

Edge Maestro **does not include** any third-party SDKs, ad networks, analytics, or crash reporting libraries. The app's only runtime dependencies are AndroidX/Jetpack libraries from Google (Compose, DataStore, Hilt, etc.) for app structure, none of which transmit user data.

### 6. Children's privacy

Edge Maestro is not directed at children under 13. The app does not knowingly collect any data from anyone, including children.

### 7. Changes to this policy

This policy may be updated as the app evolves. Updates are reflected by changing the "Last updated" date at the top.

### 8. Contact

Questions about this policy can be filed as an issue at the project's site repository:
[github.com/my13each/EdgeMaestro_Page/issues](https://github.com/my13each/EdgeMaestro_Page/issues)

---

<a id="japanese"></a>

## 日本語

### 要約

Edge Maestro は **データを一切収集・送信・共有しません**。すべての情報は端末内にのみ保存されます。

### 1. 収集する情報

**なし。** Edge Maestro は個人情報、利用データ、テレメトリ、クラッシュレポート、解析データを一切収集しません。

### 2. 端末内に保存される情報

ジェスチャー設定、アクション設定、表示設定は Android の DataStore を使用して端末内にローカル保存されます。これらのデータは:

- 端末内のみに保持される
- クラウド同期・バックアップは行われない (`allowBackup` 無効)
- いかなる外部にも送信されない
- システム設定からアプリのデータを消去するか、アプリをアンインストールすれば完全に削除できる

### 3. ネットワーク利用

Edge Maestro はインターネットを使用しません。アプリマニフェストで `INTERNET` 権限を **宣言していない** ため、Android 自体がアプリのネットワーク接続をブロックします。これはマニフェストから検証可能です。

### 4. 権限と必要理由

| 権限 | 理由 |
|---|---|
| 他のアプリの上に重ねて表示 (`SYSTEM_ALERT_WINDOW`) | エッジジェスチャーオーバーレイを他のアプリの上に描画するため。 |
| フォアグラウンドサービス (`FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_SPECIAL_USE`) | サービス動作中にジェスチャー検出を確実に継続させるため。 |
| ユーザー補助サービス (`BIND_ACCESSIBILITY_SERVICE`) | 設定したアクション (戻る・ホーム・最近のアプリ・タッチ操作) を実行するため。Edge Maestro は画面テキストを読み取ったり、パスワードを取得したり、ユーザー入力を記録することは **ありません**。Accessibility API はユーザー起動のアクション実行にのみ使用されます。また、入力中にトリガー領域がソフトキーボードと重ならないよう、ソフトキーボード (IME) ウィンドウの画面位置 (`bounds.top`) のみを読み取ります — ウィンドウのテキスト・UI 要素・入力内容には一切アクセスしません。 |
| 通知 (`POST_NOTIFICATIONS`) | Android 13 以降で必須となるフォアグラウンドサービス通知を表示するため。 |
| 起動時の自動再開 (`RECEIVE_BOOT_COMPLETED`) | 設定で有効にした場合、再起動後にサービスを再開するため。 |
| インストール済みアプリの照会 (`<queries>`) | ジェスチャーから起動するアプリを選択できるよう、ランチャー対応アプリ一覧を取得するため。一覧はローカルで読み取られるのみで、外部に送信されることはありません。 |

### 5. 第三者サービス・SDK

Edge Maestro はサードパーティの SDK、広告ネットワーク、解析ツール、クラッシュレポートライブラリを **一切組み込んでいません**。アプリのランタイム依存は Google の AndroidX/Jetpack ライブラリ (Compose、DataStore、Hilt 等) のみで、これらもユーザーデータを送信しません。

### 6. 子供のプライバシー

Edge Maestro は 13 歳未満を対象としていません。アプリは子供を含む誰からもデータを意図的に収集しません。

### 7. ポリシーの変更

アプリの進化に応じて本ポリシーが更新されることがあります。更新時は冒頭の「Last updated」日付が変更されます。

### 8. お問い合わせ

本ポリシーに関するご質問は、サイトリポジトリの Issue としてお寄せください:
[github.com/my13each/EdgeMaestro_Page/issues](https://github.com/my13each/EdgeMaestro_Page/issues)

---

<a id="korean"></a>

## 한국어

### 요약

Edge Maestro 는 **어떠한 데이터도 수집·전송·공유하지 않습니다**. 모든 정보는 사용자의 기기에만 저장됩니다.

### 1. 수집하는 정보

**없습니다.** Edge Maestro 는 개인정보, 사용 데이터, 텔레메트리, 크래시 리포트, 분석 데이터를 일체 수집하지 않습니다.

### 2. 기기에 저장되는 정보

제스처 매핑, 액션 설정, 표시 설정은 Android 의 DataStore 를 사용하여 기기 내부에 로컬 저장됩니다. 이 데이터는:

- 기기 내부에만 보관됨
- 클라우드 동기화·백업되지 않음 (`allowBackup` 비활성)
- 외부 어디로도 전송되지 않음
- 시스템 설정에서 앱 데이터를 지우거나 앱을 제거하면 즉시 삭제됨

### 3. 네트워크 사용

Edge Maestro 는 인터넷을 사용하지 않습니다. 앱 매니페스트에서 `INTERNET` 권한을 **선언하지 않으므로**, Android 가 앱의 네트워크 연결 시도 자체를 차단합니다. 매니페스트에서 검증 가능합니다.

### 4. 권한 및 필요 이유

| 권한 | 이유 |
|---|---|
| 다른 앱 위에 표시 (`SYSTEM_ALERT_WINDOW`) | 화면 가장자리 제스처 오버레이를 다른 앱 위에 그리기 위함. |
| 포어그라운드 서비스 (`FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_SPECIAL_USE`) | 서비스 동작 중 제스처 감지를 안정적으로 유지하기 위함. |
| 접근성 서비스 (`BIND_ACCESSIBILITY_SERVICE`) | 사용자가 설정한 액션 (뒤로/홈/최근앱/터치) 을 수행하기 위함. Edge Maestro 는 화면 텍스트를 읽거나 비밀번호를 캡처하거나 사용자 입력을 기록하지 **않습니다**. Accessibility API 는 사용자 주도 액션 실행에만 사용됩니다. 또한 입력 중 트리거 영역이 소프트키보드와 겹치지 않도록 소프트키보드 (IME) 윈도우의 화면 위치 (`bounds.top`) 만 읽으며 — 윈도우의 텍스트, UI 요소, 입력 내용에는 일체 접근하지 않습니다. |
| 알림 (`POST_NOTIFICATIONS`) | Android 13 이상에서 필수인 포어그라운드 서비스 알림 표시. |
| 부팅 시 자동 시작 (`RECEIVE_BOOT_COMPLETED`) | 설정에서 활성화한 경우 재부팅 후 서비스 재개. |
| 설치 앱 조회 (`<queries>`) | 제스처에서 실행할 앱을 선택할 수 있도록 런처 대응 앱 목록 조회. 목록은 로컬에서만 읽혀지며 외부로 전송되지 않습니다. |

### 5. 제3자 서비스 및 SDK

Edge Maestro 는 제3자 SDK, 광고 네트워크, 분석 도구, 크래시 리포트 라이브러리를 **일체 포함하지 않습니다**. 앱의 런타임 의존성은 Google 의 AndroidX/Jetpack 라이브러리 (Compose, DataStore, Hilt 등) 뿐이며, 이들 또한 사용자 데이터를 전송하지 않습니다.

### 6. 아동 프라이버시

Edge Maestro 는 13세 미만을 대상으로 하지 않습니다. 앱은 아동을 포함한 누구로부터도 데이터를 의도적으로 수집하지 않습니다.

### 7. 정책 변경

앱이 발전함에 따라 본 정책이 갱신될 수 있습니다. 갱신 시 상단의 "Last updated" 날짜가 변경됩니다.

### 8. 문의

본 정책 관련 문의는 사이트 리포지토리에 Issue 로 등록해 주세요:
[github.com/my13each/EdgeMaestro_Page/issues](https://github.com/my13each/EdgeMaestro_Page/issues)
