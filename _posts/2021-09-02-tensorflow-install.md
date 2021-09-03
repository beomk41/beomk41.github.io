---
title: " Python 3.6.2 Tensorflow 설치 방법"
excerpt_separator: "<!--more-->"
header:
teaser: 
toc: true
toc_sticky: true
categories:
  - Blog
  - Python
  - Machine Learning

tags:
  - Artificial Intelligence
  - Machine Learning
  - Python
---

## Tensorflow 

<img src="https://user-images.githubusercontent.com/81428281/131857679-18d6d210-472f-444e-a077-0d39799472bc.png" width="300" height="70"/>


TensorFlow는 Google에서 만든, 딥러닝 프로그램을 구현할 수 있게 다양한 기능을 제공해주는 라이브러리다.  

TensorFlow 자체는 C++로 구현 되어 있으며, Python, Java등 다양한 언어를 지원한다. 

하지만, 대부분의 편한 기능들이 파이썬으로 구현되기 때문에 주로 파이썬에서 개발하는 모습을 보여준다.


<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
## Python 3.6.2 설치 방법  

<img src="https://user-images.githubusercontent.com/81428281/131857758-3e72338d-298f-4446-a177-46265c33b872.png" width="300" height="70"/>


<https://www.python.org/downloads/windows/>



<img src="https://user-images.githubusercontent.com/81428281/131852239-434f1aa5-7328-4585-b441-0b04fc880c7b.png" width="680" height="400"/>




해당 이미지에서 자신의 운영체제에 맞는 파이썬을 설치하면 된다.

저의 경우 windows용 파이썬을 설치하기 위해 _Windows x86-64 executable installer_ 를 설치 하였습니다.

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Tensorflow 설치 방법
 
Tensorflow는 pip로 설치가 가능하며

pip script는 Python이 설치된 폴더에 위치한다.

_C:\Users\USER\AppData\Local\Programs\Python\Python36\Scripts_

pip은 Windows의 Command Window나 Linux Terminal에서 실행 할 수 있으며 다음과 같은 명령어를 이용하면  된다.  

<https://www.tensorflow.org/install>

우선 CMD나 Terminal을 실행한 뒤 명령어를 통해 pip가 위치한 디렉토리로 이동을 한다.

명령어로는 

dir : 디렉터리의 파일 및 하위 디렉터리 목록을 표시

cd (이동할 디렉토리) : 디렉터리 변경(change directory)의 준말이며, 현재의 작업 디렉터리의 위치를 변경. 

cd.. : 상위 디렉터리로 이동.

<img src="https://user-images.githubusercontent.com/81428281/131856082-711a166d-295d-4a95-8d02-f7928322dd2d.png" width="680" height="400"/>

pip가 위치하는 디렉토리까지 왔다면 다음 중 하나의 Command를 입력함으로 Tensorflow를 설치 할 수 있다.

```
Tensorflow with CPU (CPU이용)
pip install tensorflow==2.0

Tensorflow with GPU (GPU이용)
pip install tensorflow-gpu==1.15.0
```


자신이 특정 버전의 Tensorflow를 설치하고 싶다면 해당 버전을 지정해서 설치해주시면 된다.

<br/>
<br/>
<br/>

### Tensorflow 설치 확인  

Tensorflow를 설치하였다면 간단한 코드로 설치한 Tensorflow를 확인할 수 있다.

```
import tensorflow as tf
tf.__version__
```


<img src="https://user-images.githubusercontent.com/81428281/131858898-755a4b26-d876-4ff7-ad38-0f91644b7c9c.png" width="680" height="300"/>

다음 코드로 확인한 Tensorflow 버전을 업데이트 하고 싶다면 설치와 동일한 디렉토리에 들어가


다음과 같은 명령어를 입력하면 된다.

```
pip3 install --upgrade tensorflow

pip3 install --upgrade tensorflow-gpu
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

## Google colab 활용 Tensorflow 사용법

자신의 PC에 Python과 Tensorflow를 설치하지 않고 구글 Colab을 활용하여 Tensorflow를 이용하는 방법으로

<https://colab.research.google.com> 에 들어가 자신의 계정에 새 노트를 만들어 이용할 수 있다.

<img src="https://user-images.githubusercontent.com/81428281/131855232-36a48ef3-76c9-41d2-8000-a7820fc18b55.png" width="680" height="500"/>



새 노트를 만들었다면 파이썬에서 Tensorflow를 확인 하였던것 처럼 Tensorflow의 버전을 확인해 볼 수 있다.


<img src="https://user-images.githubusercontent.com/81428281/131855365-6bed320b-a8e5-4b59-835b-70d669b088dd.png" width="680" height="300"/>



