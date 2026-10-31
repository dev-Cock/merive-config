# merive-config

메리브 iOS 앱이 실행할 때 읽는 공개 설정 파일입니다.

- `version.json`
  - `minimumVersion`: 이보다 낮은 버전의 앱은 업데이트 안내 화면을 띄웁니다.
    앱은 App Store에 실제로 그 버전 이상이 올라와 있을 때만 막으므로, 이 값을 잘못 올려도 사용자가 갇히지 않습니다.
  - `message`: 업데이트 화면에 보여 줄 문구 (없으면 `null` → 기본 문구)

강제 업데이트가 필요할 때: 새 버전이 App Store에 **출시된 뒤** `minimumVersion`만 올리면 됩니다.
