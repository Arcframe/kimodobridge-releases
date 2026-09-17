# Kimodo Bridge — Releases

**In-editor Kimodo SOMA motion authoring for Unreal Engine** — by [Arcframe Inc.](https://arcframe.kr)

이 저장소는 **프리빌드 플러그인 배포 전용**입니다. 소스 코드는 포함하지 않습니다. 최신 zip은 [Releases](../../releases)에서 받으세요.

## 설치

1. `KimodoBridge-vX.Y.Z-UE5.8-Win64.zip`을 내려받아 압축을 풉니다.
2. `KimodoBridge` 폴더를 프로젝트의 `Plugins/` 아래에 넣습니다. (없으면 `Plugins` 폴더를 만듭니다.)
3. 프로젝트를 열고 Edit → Plugins에서 **Kimodo Bridge**가 켜져 있는지 확인합니다.
4. Window → **Kimodo Motion**을 열고 **서버 연결**에서 Bridge API 주소와 사용자 토큰을 입력합니다.
5. **새 모션 작업**으로 SOMA 캐릭터를 배치하고 생성·편집합니다.

SOMA 원본 캐릭터, 스켈레톤, SOMA→MetaHuman IK Retargeter는 플러그인 `Content/`에 포함되어 있어 별도 준비가 필요 없습니다. MetaHuman으로 내보낼 때만 Project Settings → Plugins → Kimodo Bridge에서 **MetaHuman Target Mesh**와 **MetaHuman Control Rig**를 프로젝트의 MetaHuman 에셋으로 지정합니다.

## 요구 사항

- Unreal Engine **5.8** (Win64)
- Bridge API 서버(`Service/` 폴더의 `kimodo_bridge.py`, 별도 GPU 환경)
- MetaHuman 내보내기 시 MetaHuman Character 플러그인

## 사용 안내

플러그인 폴더의 `README.md`, `WORK_LEVELS.md`, `START_MOTIONS.md`, `Service/README-LAN.md`를 참고하세요.

## 라이선스

Apache License 2.0. 별도로 설치하는 Unreal Engine, Kimodo, SOMA 및 모델·캐릭터 에셋에는 각 제공자의 조건이 적용됩니다.
