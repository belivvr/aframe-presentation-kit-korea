# 에이프레임 프리젠테이션-키트

A-Frame 에 대한 강연 및 프리젠테이션을 위한 공식 시작 슬라이드.

[슬라이드 보기.](https://aframe.io/aframe-presentation-kit/#/)

## 설치

1. [저장소 다운로드 하기. (.ZIP)](http://github.com/aframevr/aframe-presentation-kit/zipball/master) (>200MB)
2. node.js npm 명령어 사용. (`npm run start`)
3. 브라우저에서 호스트 사용. [ http://localhost:8080 ] 

## 목차

- 소개
- 가상현실
  - 하드웨어
  - 가상현실 생태계
- WebVR
  - 장점
  - API
  - 브라우저
  - 메타버스
  - 진입 장벽
- A-Frame
  - 소개
  - Hello World
  - 실시간 구현
  - 모든것을 함께 작동
- 자주 사용되는 시스템
  - 개념
  - 도면요소 구성
  - 레지스트리
  - 검사기
- 커뮤니티
  - 예시
  - 숫자

## 수정중인 디자인

이 키트는 [reveal.js](https://github.com/hakimel/reveal.js/) HTML 프레젠테이션 프레임워크 입니다. 
사용자 정의를 하려면, [문서화](https://aframe.io/docs/1.2.0/components/position.html#sidebar)
을 읽어 보면서 슬라이드 데크를 수정을 하세요.

스타일링은, 키트의 테마가 들어있는 자바스크립트 저장소는 흰색 테마 배경을 바탕으로 합니다. 
복사된 `src/main.css` 이 파일은 사용자가 수정하여 교체할수 있다.
--크롱--

## 내용 수정

**content.md** 파일을 수정하여 내용은 편집합니다. 슬라이드는 마크다운으로 작성되고
하이픈 6개로 구분됩니다. `------`. 사용자 또한 하이픈을 3개로 구분하여
수직 슬라이드를 추가 할 수도 있습니다. `---`. 슬라이드는 수직 슬라이드를 사용하여
드롭다운 하거나 일반적인 포인트를 기반으로 그룹화 됩니다. 당신은 각 슬라이드의 
`<!-- NOTES -->`아래에 내용을 넣어서 스피커 노트를 추가 할 수 있습니다.

사용자들에 맞게 콘텐츠를 제작합니다. 이 질문들의 대한 답변에 따라 슬라이드를 필터링
합니다. (할당된 대화 길이도 포함) 예시.

- **사용자들은 가상현실에 익숙합니까?** - 그렇다면, 가상현실 부분을 건너뛰거나 잘라 낼 수 있습니다.
- **사용자들이 기본코드 (즉, 자바스크립트, A-frame 구성요소, three.js)? 에 관심이 있습니까?** - 그렇지 않으면 도면요소-구성요소-부분을 자릅니다.

### A-frame 장면 추가

A-frame 장면이 슬라이드 바로 안에 내장되어 있어 다른 곳으로 이동할 필요 없이
데모를 할 수 있습니다. 키트가 인식할 것 입니다 `<div
data-aframe-scene="scenes/yourscene.html"></div>` 및 A-frame 장면에 들어갑니다.

## 전개

 **GitHub Pages** 및 *Source* 아래의 GitHub 저장소 설정 페이지에서
`master branch`를 선택하십시오. 그런 다음 Github 저장소로 푸쉬 하기만 하면, 슬라이드가
`https://yourusername.github.io/aframe-presentation-kit` 또는 레파지토리 이름을
지정한 위치에서 라이브 됩니다. [GitHub 페이지에 대해 자세히
알아보기](https://github.com/blog/2228-simpler-github-pages-publishing).

## 제공하다

네트워크 성능을 향상 시키려면 슬라이드를 컴퓨터에서 로컬로 제공하십시오.

사용자의 키보드의 'f' 키를 눌러 전체 화면으로 이동합니다. 사용자의 키보드의 `s` 키를 
눌러 **Speakers Notes** 창을 엽니다. 축소된 슬라이드 개요를 보려면
사용자의 키보드의 'esc' 또는 'o' 키를 누릅니다.

내장된 A-frame 장면이 있는 슬라이드가 있습니다. 슬라이드 바로 안쪽에서 부터 실시간으로
이 장면들을 재생합니다. 클릭하여 드래그하면 둘러 볼 수 있습니다. 사용자 전체화면으로
들어가거나 헤드셋이 연결된 경우 VR로 들어갈 수 있습니다.

사용자의 키보드의 `<ctrl> + <alt> + i`를 눌러 A-frame 관리자의 한 장면을 
엽니다. 이렇게 하면 시각적 도구에 포함된 A-frame 장면이 열릴 것 입니다.

이것 좀 보세요 [public speaking guide](http://speaking.io/) 그리고 행운을 빌어요!
--루피--
