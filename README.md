# Chiikawa Pet Installer

![Chiikawa pet preview](plugins/chiikawa-pet-installer/assets/chiikawa-idle-preview.gif)

ChatGPT Work의 Pets 라이브러리에 애니메이션 치이카와 펫을 추가하고 활성화하는 스킬형 플러그인입니다.

## 가장 쉬운 설치 방법

1. [설치용 ZIP](dist/chiikawa-pet-installer-0.1.0.zip)을 다운로드합니다.
2. 플러그인 개발자 업로드 화면이나 지원되는 로컬 마켓플레이스에 ZIP을 추가합니다.
3. 플러그인을 설치한 뒤 새 ChatGPT Work 또는 Codex 대화를 시작합니다.
4. 다음과 같이 요청합니다.

   > 번들된 치이카와 펫을 설치하고 선택해줘.

공식 ChatGPT Pets 기능과 Pets 도구를 사용할 수 있는 계정이어야 합니다. 각 사용자의 Pets 라이브러리에 별도 소유 복사본이 생성되며, 이 저장소에는 원 제작자의 펫 ID, 업로드 세션, 계정 정보가 포함되지 않습니다.

## GitHub 마켓플레이스로 설치

Codex CLI에서 이 저장소를 마켓플레이스로 추가할 수 있습니다.

```text
codex plugin marketplace add 1ny/chiikawa-pet-installer
```

그다음 ChatGPT 데스크톱 앱을 다시 시작하고 **Plugins**에서 **Chiikawa Pet Installer**를 찾아 설치합니다.

## 저장소 구조

```text
.agents/plugins/marketplace.json
plugins/chiikawa-pet-installer/
  plugin.json
  .codex-plugin/plugin.json
  skills/install-chiikawa/SKILL.md
  assets/
dist/chiikawa-pet-installer-0.1.0.zip
```

## 안내

이 프로젝트는 비공식 팬 제작 플러그인입니다. 치이카와 및 관련 캐릭터의 권리는 각 권리자에게 있습니다.
