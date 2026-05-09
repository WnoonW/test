# DirectX 12 이미지 텍스처 렌더링 프로그램 (v2.0)

**WIC를 사용해 실제 .png / .jpg 파일을 로드해서 텍스처로 렌더링하는 프로그램**

## 기능
- WIC (Windows Imaging Component) 이미지 로드 (.png, .jpg 지원)
- 텍스처 생성 및 GPU 업로드
- 선형 필터링 + Wrap 샘플링
- 클랩(Quad) 텍스처 렌더링
- 실제 이미지 파일 지원

## 빌드 및 실행 방법

### 1. Visual Studio 프로젝트 설정
1. **C++ > Windows Desktop Application** 프로젝트 생성
2. `main.cpp` 파일 드랩
3. **프로젝트 속성** → **링커** → **시스템** → **하위 시스템** = **Windows (/SUBSYSTEM:WINDOWS)**
4. 빌드 (F7)

### 2. 이미지 파일 준반
- 프로젝트 폴더(또는 .exe 가 있는 폴더)에 **`test.png`** 파일을 넣어주세요.
- 파일 이름을 바꾸고 싶으면 `main.cpp` 안의 `LoadTextureFromFile(L"test.png", ...)` 라인을 수정하세요.

### 3. 실행
F5 또는 빌드 후 .exe 실행

## 실행 결과
원하는 이미지가 중앙에 클랩 형태로 렌더링됩니다!

## 파일 구성
- `main.cpp` — 전체 소스 코드 (WIC + DirectX 12 텍스처)
- `README.md` — 이 설명서

## 기술 점
- WIC 로더 사용 (외부 라이브러리 미필요)
- Upload Heap → Default Heap 전송
- Static Sampler 사용
- Shader Resource View (SRV) 바인딩

**Made with ❤️ by Grok for WnoonW**