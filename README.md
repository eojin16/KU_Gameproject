# KU_GameProject

고려대학교 2023년 실용 SW 프로젝트 수업 결과물입니다.

## 📖 프로젝트 개요

이 프로젝트는 Unity 엔진을 사용하여 절차적 던전 생성(Procedural Dungeon Generation) 알고리즘을 구현한 게임 프로젝트입니다. 다양한 알고리즘을 통해 매번 다른 형태의 던전을 자동으로 생성할 수 있습니다.

## 🎮 주요 기능

### 던전 생성 알고리즘

프로젝트는 세 가지 주요 던전 생성 방식을 구현합니다:

1. **Simple Random Walk (단순 랜덤 워크)**
   - 시작점에서 랜덤하게 이동하며 던전을 생성
   - 유기적이고 자연스러운 동굴 형태의 던전 생성

2. **Room First (방 우선 생성)**
   - 먼저 방들을 배치한 후 복도로 연결
   - 구조적이고 계획된 던전 레이아웃

3. **Corridor First (복도 우선 생성)**
   - 복도를 먼저 생성한 후 방을 배치
   - 미로 같은 복잡한 던전 구조

### 시각화 시스템

- **Tilemap Visualizer**: Unity Tilemap 시스템을 활용한 던전 시각화
- **Wall Generator**: 자동 벽 생성 및 타입 분류
- **Wall Types Helper**: 벽의 방향과 연결 상태에 따른 타일 선택

## 🗂️ 프로젝트 구조

```
Assets/
├── _Scripts/               # 스크립트 파일
│   ├── Data/              # 데이터 관련 스크립트
│   ├── AbstractDungeonGenerator.cs
│   ├── SimpleRandomWalkDungeonGenerator.cs
│   ├── RoomFirstDungeonGenerator.cs
│   ├── CorridorFirstDungeonGenerator.cs
│   ├── ProceduralGenerationAlgorithms.cs
│   ├── TilemapVisualizer.cs
│   ├── WallGenerator.cs
│   └── WallTypesHelper.cs
├── _Sprites/              # 스프라이트 리소스
├── Scenes/                # Unity 씬 파일
├── Tiles/                 # 타일 에셋
├── Resources/             # 리소스 파일
└── Editor/                # 에디터 확장 스크립트
```

## 🛠️ 기술 스택

- **Engine**: Unity
- **Language**: C#
- **Graphics**: Unity Tilemap System

## 🚀 시작하기

### 필요 조건

- Unity (2020.3 이상 권장)
- Visual Studio 또는 기타 C# IDE

### 설치 및 실행

1. 저장소 클론
```bash
git clone https://github.com/eojin16/KU_Gameproject.git
```

2. Unity Hub에서 프로젝트 열기
   - Unity Hub 실행
   - "Add" 버튼 클릭
   - 클론한 프로젝트 폴더 선택

3. Unity에서 프로젝트 실행
   - Scenes 폴더의 씬 파일 열기
   - Play 버튼을 눌러 실행

## 📚 알고리즘 설명

### Procedural Generation Algorithms

프로젝트의 핵심 알고리즘들은 `ProceduralGenerationAlgorithms.cs`에 구현되어 있습니다:

- **Random Walk**: 랜덤한 방향으로 이동하며 경로 생성
- **BSP (Binary Space Partitioning)**: 공간을 재귀적으로 분할하여 방 생성
- **Cellular Automata**: 셀룰러 오토마타 규칙을 활용한 동굴 생성

### Abstract Pattern

`AbstractDungeonGenerator`를 상속받아 각 생성 방식을 구현함으로써 확장 가능한 구조를 유지합니다.

## 👥 기여

고려대학교 실용 SW 프로젝트 수업의 결과물입니다.

## 📝 라이선스

이 프로젝트의 라이선스 정보는 별도로 명시되지 않았습니다.

## 📧 문의

프로젝트 관련 문의사항이 있으시면 GitHub Issues를 통해 연락주세요.

---

**Last Updated**: June 3, 2023
