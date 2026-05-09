# DirectX 12 이미지 렌더링 프로그램

이 프로젝트는 **DirectX 12** 를 사용하여 간단한 이미지를 렌더링하는 Windows 응용 프로그램입니다.

## 기능
- Windows 웰도우 생성
- DirectX 12 기기 초기화 (Device, SwapChain, Command Queue)
- 색상 삼각형 (Colored Triangle) 렌더링
- 텍스처 지원 확장 가능

## 빌드 및 실행 방법

### 필수 요구 사항
- Windows 10 / 11
- Visual Studio 2022 (Desktop Development with C++)
- Windows 10 SDK (또는 최신)

### 빌드 스텝
1. Visual Studio 실행
2. 새 프로젝트 생성: **C++ > Windows Desktop Application**
3. `main.cpp` 파일을 프로젝트 폴더에 드랩
4. 빌드 (F7) 및 실행 (F5)

## 실행 화면
파란색 배경에 색상 삼각형 (Red-Green-Blue) 이 렌더링 됩니다!

## 파일 구성
- `README.md` - 이 설명서
- `main.cpp` - 주 소스 코드 (DirectX 12 기본 렌더링)

## 다음 단계 (TODO)
- 이미지 텍스처 로드 및 렌더링
- 회전 / 애니메이션
- 스크롤 바

이 코드는 기본적인 DirectX 12 파이프라인을 구현했습니다. 실제 이미지를 렌더링하려면 텍스처 리소스를 추가하세요 (WIC 또는 stb_image 사용 권장).

**Made with ❤️ by Grok for WnoonW/test repo**