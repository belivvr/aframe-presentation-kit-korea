<!-- .slide: data-background="media/img/aframe.jpg" -->

<div class="talk-title">
  <h1>에이-프레임</h1>
  <p>가상현실 환경을 구축하기 위한 웹 프레임워크</p>
  <p class="talk-info">
    @belivvr | Mozilla VR | **afrmae.io-kr**
  </p>
</div>

<!-- NOTES -->
- 3D 및 VR 세계로 웹 개발자들이 온보드를 해줍니다.
- 더 빠른 경험담을 웹VR 프로토타입을하세요.

------

# 가상 현실

<!-- .slide: data-background-video="media/video/virtualreality.mp4" data-background-video-loop="true" data-background-video-muted="true" data-state="state--bg-dark" -->

<!-- NOTES -->
- 물어보세요! VR을 얼마나 많이 경험을 해봤는지
- 가상 현실은 기술 플랫폼이며 현실적이고 상호적이며, 몰입감 있는 3D 환경으로 사용자를 이동시킵니다.
- 다음 플랫폼은 작업 방식을 바꿀 것입니다. 디지털 방식으로 재생하고 소통하고, 사회의 얼굴입니다.

---

<div class="image-row">
  <div><img data-src="media/img/google-cardboard.png"></div>
  <div><img data-src="media/img/google-daydream.png"></div>
  <div><img data-src="media/img/samsung-gearvr.png"></div>
</div>

<div class="image-row">
  <div><img data-src="media/img/oculus-rift.png"></div>
  <div><img data-src="media/img/playstation-vr.png"></div>
  <div><img data-src="media/img/htc-vive.png"></div>
</div>

<!-- NOTES -->
- 백앤드는 모든 기업에서 크게 원합니다.
- 저렴한 것부터 비싼 것까지, 테더링 및 언테더링, 컨트롤러, 추적 다양한게 많습니다.
- Steam이 제공하는 HTC Vive는 현재 가장 매력적인 경험을 제공합니다.
- 보세요! 많고 다른 디바이스,시스템.플랫폼등 서로 경쟁을 합니다...

---

## 가상현실의 생태계

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/gatekeeper.png">
    <i>문지기</i>
  </div>
  <div>
    <img data-src="media/img/downloads-installs.png">
    <i>다운</i>
  </div>
  <div>
    <img data-src="media/img/closed-door.png">
    <i>닫힘</i>
  </div>
</div>

<!-- NOTES -->
- 앱스토어 및 기업들이 배포를 하며 제어합니다 : 콘텐츠를 게시 중단하거나 차단할 수 있습니다.
- 다운로드 / 설치하는데의 소비는 용량 : 작은 비지니스 페이지.
- 생태계 폐쇠 : 소유권을 가진 유저, 가파른 학습 곡선, 고립된 경험, 분열 등이 있습니다.
- 우리는 VR이 성공하길 바라기 때문에 이러한 마찰이 없는 플랫폼을 원합니다. 정답은 WebVR입니다...

------

# 웹 가상현실

개방형 가상 현실 플랫폼의 ** 웹의 ** 장점

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/web-is-open.png">
    <i>개방적</i>
  </div>
  <div>
    <img data-src="media/img/web-is-connected.png">
    <i>연결</i>
  </div>
  <div>
    <img data-src="media/img/web-is-instant.png">
    <i>즉각적</i>
  </div>
</div>

<!-- NOTES -->
웹VR은 브라우저의 가상 현실로 인터넷을 기반으로 합니다.

열다:
- 공개적으로 누구나 만들수있습니다.
- 개방형 오픈소스 문화.

연결:
- 트래버스 월드.

즉각적:
- 한번의 클릭으로 트위터,시나 웨이보 등 즉각적인 VR 경험담을 들을수 있다.
- 설치를 하지 않음.
- 상상해보세요! VR로 쇼핑과 개인 공간을.
- 좋은 경험을 하실 수 있습니다.

전환:
- 웹은 사람들을 위한 최고의 플랫폼으로 만드는 장점을 가지고 있습니다.
- 현실화하기 위해 행동해야 하고, VR이 구워지고 결정화되기를 기다릴 수 없다.
- 관여하다.

---

<img class="stretch" data-src="media/img/webvr.png">


브라우저 API는 WebGL이랑 렌더링 하게끔 할 수 있으며 헤드셋과 허용된 VR기기가 있으면 됩니다.

https://w3c.github.io/webvr/

<!-- NOTES -->
API:
- 헤드셋의 렌더링 경로 최적화합니다.
- 액세스 위치 및 회전(포즈) 데이터

역사:
- 초기 웹VR API는 모질라가 만들었습니다.
- W3C 커뮤니티 그룹과 작업을 하였습니다.
- 모질라, 구글, 삼성, 마이크로소프트 커뮤니티는 현재 웹VR 1.0 API를 사용하고 있습니다.

단순한 사양이 아니라 구현됌..

---

https://webvr.rocks

<div class="captioned-image-row small">
  <div>
    <img data-src="media/img/firefox-nightly.png">
    <i>파이어폭스 <br>나이틀리</i>
  </div>
  <div>
    <img data-src="media/img/edge.jpg">
    <i>마이크로소프트 <br>엣지</i>
  </div>
  <div>
    <img data-src="media/img/chromium.png">
    <i>크로미엄</i>
    <i></i>
  </div>
</div>

<div class="captioned-image-row small">
  <div>
    <img data-src="media/img/chrome.jpg">
    <i>안드로이드용 크롬</i>
    <!-- <i>크롬</i> -->
  </div>
  <div>
    <img data-src="media/img/carmel.jpg">
    <i>오큘러스 <br>카멜</i>
  </div>
  <div>
    <img data-src="media/img/samsung-browser.png">
    <i>삼성<br> 인터넷</i>
  </div>
  <div>
    <img data-src="media/img/google-cardboard.png">
    <i>모바일<br> 폴리필</i>
  </div>
</div>

<!-- NOTES -->
- 파이어폭스 + 크롬 웹VR 1.0 2017 2017년 초까지 히트 출시 채널 이였습니다.
- 현재  Nightly는 사용자 정의 빌드 및 플래그를 하고있습니다
- 모바일 폴리필: 디바이스 동작 / 방향 센서 - 스마트폰에서 폴리필에 있음.
- 모든 브러우저 뒤에...

---

## 메타버스

<!-- .slide: data-background="media/img/metaverse.jpg" -->

<!-- NOTES -->
- 공유 영구 집합 가상 공간
- 세상이 살고, 일하고, 놀 수 있는 디지털 현실을 대체하세요.
- 분산/개방/연결되어야 하며, 웹은 완벽하게 실현하기 위한 최상의 플랫폼입니다.
- 어디서부터 시작할까요?
- three.js abstracts WebGL, 3D 들과 웹VR 을 추상화 하면 접근성을 높일 수 있습니다.

---

웹가상현실을 만들기가 너무 어렵습니다...

---

<!-- .slide: data-background-video="media/video/boilerplate.mp4" data-state="state--bg-dark" -->

<div class="slide__boilerplate">
  <p>웹가상현실에서 폴리필을 가져오세요.</p>
  <p>카메라 설정</p>
  <p>조명 설정</p>
  <p>씬 초기화</p>
  <p>넘어갈 캔버스를 선언</p>
  <p>사운드 창 크기 조절</p>
  <p>VR임팩트 설치</p>
  <p>렌더러 인스턴스화</p>
  <p>렌더 루프 만들기</p>
  <p>프리팹 에셋</p>
  <p>응답성 파악</p>
  <p>메타태그 및 모바일 처리</p>
</div>

<!-- NOTES -->
- WebVR 환경을 만드는 것은 너무 어렵습니다.
- 작은 프로토타입을 실험을 하는 경우 큰 장애물이 있습니다
- 보일러 플레이트는 웹VR, three.js 및 브라우저의 단점이 있어 새 버전으로 업데이트해야 합니다
- 모든걸 한 줄로 캡슐화 시킵니다.

------

# 에이-프레임

<!-- .slide: data-background="media/img/aframe-rendered-full.png" -->

하나의 웹 프레임워크를 위한 가상 현실 구축 경험담

<!-- NOTES -->
- 작년 12월 출시
- 이유:
  - 웹 개발자가 그래픽 지식 없이도 VR 콘텐츠를 쉽게 만들 수 있습니다.
  - 웹VR 및 VR UX 프로토타입 및 실험 속도가 향상이 됩니다.
  - 웹VR 생태계를 시작하는 수단

---

## 코딩 해보기

<!-- .slide: data-background="media/img/aframe.jpg" data-transition="slide-in none" -->

```html
<html>
  <script src="https://aframe.io/releases/0.5.0/aframe.min.js"></script>
  <a-scene>





  </a-scene>
</html>
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- HTML 만으로.
- 스크립트 태그 삭제, 빌드 단계 없음.
- 사용자가 HTML을 지정해서 사용할 수 있음.
- HTML `<a-scene>` 한줄로 부터 시작합니다. 
  - 캔버스, 카메라 , 렌더러, 빛 , 조작 , 렌더루프 , 웹VR 폴리필, VR이팩트
- 장면 안에 재료를 넣으세요.

---

## 코딩 해보기

<!-- .slide: data-background="media/img/aframe.jpg" data-transition="fade-in slide-out" -->

```html
<html>
  <script src="https://aframe.io/releases/0.5.0/aframe.min.js"></script>
  <a-scene>
    <a-box color="#4CC3D9" position="-1 0.5 -3" rotation="0 45 0"></a-box>
    <a-cylinder color="#FFC65D" position="1 0.75 -3" radius="0.5" height="1.5"></a-cylinder>
    <a-sphere color="#EF2D5E" position="0 1.25 -5" radius="1.25"></a-sphere>
    <a-plane color="#7BC8A4" position="0 0 -4" rotation="-90 0 0" width="4" height="4"></a-plane>
    <a-sky color="#ECECEC"></a-sky>
  </a-scene>
</html>
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- 기초적인 3D 기본요소를 사용자 정의를 해보세요.
- 가독성 : HTML은 가장 접근하기 쉬운 언어입니다.
- 캡슐화: 다른 곳에서 HTML을 복사하여 붙여넣고 상태 또는 변수 없이 계속 작동합니다.
- 빠르게 보며 만들어보세요!

---

## 안녕! 메타버스

<i>by belivvr (@belivvr)</i>

<!-- .slide: data-background="media/img/metaverse.jpg" -->

<div class="stretch" data-aframe-scene="scenes/80s.html"></div>

<!-- NOTES -->
- HTML 안에서 실행되는 빌리버의 에이-프레임
- 데스크탑, 안드로이드, 아이오에스, 삼성 기어VR, 오큘러스 Rift, HTC Vive에서 일을 할수 있다.
- 돔 인스펙터를 열어 값을 실시간으로 변경할 수 있습니다.

---

# 개체(entity)-요소-시스템

<!-- .slide: data-background="media/img/minecraft-blocks.png" -->

<!-- NOTES -->
- 객체-요소에 대한 프레임워크
- 인기있는 게임개발, 유니티를 사용합니다.
- 씬(Scene)의 모든 개체는 기본적으로 빈 개체인 **entity**입니다.
  모양을 첨부할 **구성요소** | 행동 | 기능성
- 2D 웹은 모든 요소가 고정되어있다.
- 3D/VR은 다르다, 무한적인 유형 및 복잡성을 가진 객체에는 다양한 종류의 객체를 쉽게 구축할 방법이 필요합니다.

---

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="slide-in none" -->

## 도면요소 구성

```html
<a-entity>
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- `<a-entity>` 적어보세요!
- 이 상태로는 외관, 행동, 기능이 없습니다.
- 구성 요소를 연결하여 모양, 동작, 기능 추가합니다.

---

## 도면요소 구성

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  geometry="primitive: sphere; radius: 1.5"
  material="color: #343434; roughness: 0.4; sphericalEnvMap: #texture">
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- CSS스타일과 비슷합니다.
- HTML 속성으로 구성 요소 이름을 만듭니다.
- HTML 속성 값으로서의 구성 요소 속성 및 값이 생성됩니다.

---

## 도면요소 구성

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  geometry="primitive: sphere; radius: 1.5"
  material="color: #343434; roughness: 0.4; sphericalEnvMap: #texture"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2">
```
<!-- .element: class="stretch" -->

---

## 도면요소 구성

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  geometry="primitive: sphere; radius: 1.5"
  material="color: #343434; roughness: 0.4; sphericalEnvMap: #texture"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2"
  animation="property: rotation; loop: true; to: 0 360 0"
  movement-pattern="type: spline; speed: 4">
```
<!-- .element: class="stretch" -->

---

## 도면요소 구성

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  json-model="src: #robot"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2"
  animation="property: rotation; loop: true; to: 0 360 0"
  movement-pattern="type: spline; speed: 4">
```
<!-- .element: class="stretch" -->

---

## 도면요소 구성

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  json-model="src: #robot"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2"
  animation="property: rotation; loop: true; to: 0 360 0"
  movement-pattern="type: attack; target: #player"
  explode="on: hit">
```
<!-- .element: class="stretch" -->

---

<!-- .slide: data-background="media/img/standard-components.png" data-background-size="contain" -->

<!-- NOTES -->
- 에이-프레임과 함께 제공되는 일부 구성 요소입니다
- 에이-프레임은 확장이 가능하며, 핵심이 됩니다.

---

<!-- .slide: data-background="media/img/community-components.png" data-background-size="contain" -->

<!-- NOTES -->
- 커뮤니티는 수많은 구성요소로 생태계를 가득 채웠습니다.
- 구성요소는 원하는 모든 작업을 수행할 수 있으며, three.js 및 웹 API에 대한 전체 액세스 권한을 갖습니다.
- 에이-프레임의 생명줄인 구성요소 생태계입니다.
- 물리학, 립모션, 입자 시스템, 오디오 시각화, 해양 등 있습니다.
- 구성 요소를 스크립트 태그로 삭제하고 HTML에서 직접 사용합니다.
- 고급 개발자가 다른 개발자에게 권한을 부여합니다.
- 구성 요소 수집 작업중 입니다.

---

# 레지스트리

<!-- .slide: data-background-color="#333" -->

큐레이션된 A-Frame 구성요소 모음입니다.

<a class="stretch" href="https://aframe.io/aframe-registry">
  <video loop data-src="media/video/registrypreview.mp4" data-autoplay></video>
</a>

<!-- NOTES -->
- 에이-프레임 레지스트리 수집을 합니다.
- 잘 작동하도록 하는 부품 저장소처럼.
- 사용자는 구성요소를 찾아 검색하거나 설치할 수 있습니다.

---

# 레지스트리

<!-- .slide: data-background-color="#333" -->

큐레이션된 A-Frame 구성요소 모음입니다.

<video loop data-src="media/video/leaphands.mp4" data-autoplay></video>

---

## Inspector

<!-- .slide: data-background="media/img/inspector.png" data-state="state--bg-dark" -->

Visual tool for A-Frame. Just `<ctrl>+<alt>+i`.

<div class="stretch" data-aframe-scene="scenes/80s.html"></div>

------

<!-- .slide: data-background="media/img/header.png" -->

# 커뮤니티

https://aframe.io/blog/

---

<!-- .slide: data-background="media/img/apainter.gif" -->

# Art - *A-Painter*

@mozillavr

---

<!-- .slide: data-background="media/img/syria.gif" -->

# Journalism - *Fear of the Sky*

Amnesty International UK

---

<!-- .slide: data-background="media/img/mars.jpg" -->

# Journalism - *Journey to Mars*

The Washington Post

---

<!-- .slide: data-background="media/img/citybuilder.gif" -->

# Sandbox - *City Builder*

@kfarr

---

<!-- .slide: data-background="media/img/adit.gif" -->

# Data Visualization - *Adit*

@datatitian

---

<!-- .slide: data-background="media/img/a-blast.gif" -->

# Gaming - *A-Blast*

@mozillavr

---

<!-- .slide: data-background="media/img/ux.gif" -->

# Prototyping - *UI Widgets*

@whoyee

---

<!-- .slide: data-background="media/img/math.gif" -->

# Mathematics - *MathworldVR*

@sleighdogs

---

<!-- .slide: data-background="media/img/ar.gif" -->

# AR - *AR.js + A-Frame*

@jerome_etienne

---

<!-- .slide: data-background="media/img/webvrstudio.png" -->

# Tools - *WebVR Studio*

@webvrstudio

---

<!-- .slide: data-background-video="media/video/livetour.mp4" data-background-video-loop="true" -->

# Real Estate - *Live Tour*

iStaging

---

<!-- .slide: data-background="media/img/cadavr.gif" -->

# Education - *CadaVR*

@drryanjames

---

# aframe.io

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/github.png">
    <i>180+ contributors 6000+ Stargazers</i>
  </div>
  <div>
    <img data-src="media/img/slack.png">
    <i>4000+ members on Slack</i>
  </div>
  <div>
    <img data-src="media/img/scene-collage-circle.png">
    <i>100s of featured projects</i>
  </div>
</div>

<!-- NOTES -->
- Open source and inclusive project
- Most work done on GitHub
- Active community on Slack to share projects, interact, hang out, seek help
- Featured projects on the `awesome-aframe` repository and *A Week of A-Frame* blog
