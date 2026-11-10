# DX3DStart — Game Tech Lab Week 02

DirectX 11로 처음 진입한 주차입니다. 렌더링 파이프라인을 직접 세우고, MVP 변환과 카메라를 구현한 뒤 회전 표현을 쿼터니언으로 정리했습니다.

## 내가 맡은 부분 — 신동민

**기간** 2025.09.05 – 09.10 · **팀** 4인 · **내 커밋** 34건

| 구현 | 내용 |
| --- | --- |
| **MVP 변환** | MVP 구현, 오른손 좌표계로 정리, CPU 측에서 행렬 곱 수행 |
| **카메라** | 키보드 이동 + 마우스 회전 입력 구현 |
| **쿼터니언** | `Quaternion` 자체 구현, 쿼터니언↔오일러 변환 헬퍼, 카메라와 오브젝트 회전을 모두 쿼터니언으로 전환한 뒤 리팩토링 |
| **뷰포트** | 창 크기 변경 시 비율을 유지해 화면이 늘어나거나 찌그러지지 않도록 처리, 초기 실행 시 렌더되지 않던 문제 해결 |
| **기즈모** | 기즈모 모드 선택 |

**주요 파일** `Engine/Quaternion.h` · `Engine/Camera.h` · `Engine/Matrix.h` · `Engine/UGizmoManager.cpp`

→ **[내 커밋 34건 보기](https://github.com/TeshShin/Krafton_TechLab_Week02/commits?author=TeshShin)** · [주차 학습 노트](https://app.notion.com/p/teshstudy/2-2D-to-3D-Core-System-26b78d59866f800db94ee60b2e2d5844) · [14주 전체 정리](https://github.com/TeshShin/Krafton-TechLab-Roles)

---

## 이 주차 엔진에 들어간 것 (팀 전체)

- **MVP 변환 파이프라인** — 모델·뷰·프로젝션 행렬 구성, 왼손 좌표계 정리
- **카메라** — 키보드 이동, 마우스 회전 입력
- **쿼터니언 회전 체계** — 쿼터니언 자체 구현, 오일러 변환 헬퍼, 카메라·오브젝트 회전 전환
- **기즈모** — 기즈모 모드 선택
- **뷰포트 리사이즈 대응** — 창 크기가 바뀌어도 종횡비 유지

## 기술 스택

C++ · DirectX 11 · ImGui

