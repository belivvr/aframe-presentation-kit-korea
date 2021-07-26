# aframe-presentation-kit

A-Frame에 대한 강연 및 프리젠테이션을 위한 공식 시작 슬라이드.

[슬라이드 보기.](https://aframe.io/aframe-presentation-kit/#/)

## 설치

1. [Download the repository (.ZIP)](http://github.com/aframevr/aframe-presentation-kit/zipball/master) (>200MB)
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
  - Works With Everything
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
사용자 정의를 하려면, [documentation](https://aframe.io/docs/1.2.0/components/position.html#sidebar)
을 읽어 보면서 슬라이드 데크를 수정을 하세요.

스타일링은, 키트의 테마가 들어있는 자바스크립트 저장소는 흰색 테마 배경을 바탕으로 합니다. 
복사된 `src/main.css` 이 파일은 사용자가 수정하여 교체할수 있다.
--크롱--

## Modifying Content

Modify the **content.md** file to edit content. Slides are written in Markdown
and separated by six hyphens `------`. You can also add vertical slides by
separating with three hyphens `---`. The slides are grouped, using vertical
slides to drill down or build on general points. You can add speaker notes
by putting content under `<!-- NOTES -->` on each slide.

Tailor the content to your audience. Filter out slides depending on the answers
to these questions (as well as the allotted length of your talk). For example:

- **Is your audience familiar with virtual reality?** - If so, you might want to skip or trim the *Virtual Reality* section.
- **Is your audience interested in underlying code (i.e., JavaScript, A-Frame components, three.js)?** - If not, then trim the *Entity-Component-System* section.

### Adding A-Frame Scenes

A-Frame scenes are embedded right within the slides so you can demo without
having to navigate away. The kit will recognize `<div
data-aframe-scene="scenes/yourscene.html"></div>` and load in the A-Frame
scene.

## Deployment

In your GitHub repository settings page under **GitHub Pages** and *Source*,
select `master branch`. Then simply push to your GitHub repo, and then your
slides will be live at `https://yourusername.github.io/aframe-presentation-kit`
or whatever you named the repository. [Read more about GitHub
Pages](https://github.com/blog/2228-simpler-github-pages-publishing).

## Presenting

Serve the slides locally from your computer for better network performance.

Press the `f` key on your keyboard to go full screen. Press the `s` key on your
keyboard to open up the **Speakers Notes** window. Press the `<esc>` or `o` key
on your keyboard to see a zoomed out overview of the slides.

There are slides with embedded A-Frame scenes. Play with these scenes live from
right within the slide. Click and drag to look around. You may enter full
screen, or if you have a headset connected, enter VR.

Open up a scene in the A-Frame Inspector by pressing `<ctrl> + <alt> + i` on
your keyboard. This will open up an embedded A-Frame scene in a visual tool.

Check out this [public speaking guide](http://speaking.io/) and good luck!
