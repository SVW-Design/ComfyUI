# ComfyUI

Stable Diffusion
---
- Stability AI 에서 배포한 이미지 생성 AI 툴

- 오픈 소스로 누구나 사용할 수 있도록 공개

- 디지털 도화지 위의 수많은 가능성 속에서 우리가 이야기하는 말이나 그림 등을 토대로 가능성을 좁혀나가는 과정

- 장정

  - 무료
 
  - 자신의 컴퓨터에 설치하여 사용 가능
 
  - ControlNet, Lamma, IP-Adapter 등 다양한 AI 와 결합해서 다양한 기능 지원
 
  - 포토샵, 크리타, 블렌더 등 외부 프로그램과의 연동 자유로움
 
  - 빠른 발전 속도
 
    - 새로운 AI 기능이 등장하면, 1주일 내에 결합해서 사용 가능
   
  - 사용자가 자신의 취향에 따라 디테일하게 조정 가능
 
- 단점

  - 편리하게 접속해서 사용할 수 있는 미드저니(Midjourney) 등과 달리 사용자가 직접 컴퓨터에 설치해야 함
 
  - Git 이나 Python 등 툴 필요
 
    - 예전보다 쉽게 설치할 수 있는 StabilityMatrix 등 프론트엔드 툴이 등장해 사용이 편해지는 중
   
  - 생성형 AI 는 GPU 를 사용하므로, 성능이 좋은 Nvidia 기반의 그래픽카드 필수
 
<br>

|도식화|
|-|
|![이미지](./img/01.png)|
|- **Checkpoint** : 수많은 이미지의 가능성을 담고 있는 마법상자, 체크포인트에 따라 그릴 수 있는 가능성 종류가 다름<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;어떤 체포인트는 실사 가능성이 높고, 어떤 건 애니메이션이 될 가능성이 높음<br><br>- **Clip Encode & ControlNet** : 글과 그림을 기계의 말로 바꿈<br><br>- **Conditioning** : 가능성을 걸러내는 역할(채점표)<br><br>- **KSampler** : 체크포인트에 있는 수많은 가능성을 걸러내는 체 역할, Conditioning 기준으로 걸러냄<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Step : 몇 번 걸러낼지 결정하는 것<br><br>- **VAE** : 걸러진 1개의 가능성을 사람이 볼 수 있는 이미지로 변환하는 역할|

<br>

---

<br>

ComfyUI(컴피유야이)
---
- 프로그래밍 능력이 좋아야하는 Stable Diffusion 을 쉽게 사용할 수 있게 도와주는 도구

- 노드들을 연결해 기능 구현

- 매우 복잡

- 다양한 작업 수행 가능

  - **완전한 유연성** : 각 작업을 노드로 시각화하여, 자신만의 맞춤형 워크플로우 설계 가능
 
  - **빠른 업데이트** : 최신 AI 기술이 나오면 며칠 안에 커스텀 노드를 통해 바로 사용 가능
 
  - **고급 사용자에게 최적** : 창의적인 작업을 최대한 자유롭게 구현하고자 하는 사용자에게 이상적

<br>

### ComfyUI vs WebUI
|ComfyUI|WebUI|
|-|-|
|- 익숙해지기는 어렵지만, 한번 익숙해지면 자유로운 작업 가능<br>- 요리로 치면 밀가루부터 반죽하는 느낌<br>- 발전 속도가 빨라 새로운 AI 가 등장하면 2~3일 내에<br>&nbsp;&nbsp;&nbsp;ComfyUI 에 커스텀 노드로 결합되어 사용 가능|- 사용하기 쉬움<br>- 깊이 들어가면 한계 존재<br>- 요리로 치면 컵라면 or 밀키트 느낌|
