# ubuntu



### 해외뉴스 및 정보

https://telegra.ph/news-and-more-08-16



------------------------------------------------------------------------------------------------
### 한글 입력기 설치 

https://gist.github.com/leeseomin/b7eb8714d2dacaba1b3232c3c9a24113


### 우분투 필수 프로그램 세팅 

https://gist.github.com/leeseomin/b475e32a63b2cacc4177c6b8fc9f5f72


### ffmpeg 예제 

https://gist.github.com/leeseomin/1f13cd8a11fc4e772208bedbe67453b8


### 깃헙 비디오 올리기 

그냥 MP4파일  드래그 



###  youtube-dl  다운로드 예제 

https://gist.github.com/leeseomin/7c33573a053cb9a6e21257a1552f7219


### 명화 다운로드 

https://gist.github.com/leeseomin/85c60c30dc803faa865fb6f6cdd78830


### 기본 이미지 편집 명령어 

https://gist.github.com/leeseomin/be03a1b82e53b3d77e72f1a7430048ac

### 페이스 모핑

https://github.com/seominlee/Face-Morphing


### docker 설치  on ubuntu20.04

https://gist.github.com/leeseomin/55a7ee160db7fe638cc8f3ebc1119f23

### docker  예제1    이미지 캡션닝

https://gist.github.com/leeseomin/133eac0165b685041740cb03f34ce214

###  실습으로 알아보는 이미지필터  아르떼 테스트



# art history


모던아트
https://en.m.wikipedia.org/wiki/Modern_art


현대예술 

https://en.m.wikipedia.org/wiki/Contemporary_art

https://artsandculture.google.com/entity/contemporary-art/m0h0vk?hl=en


미니멀리즘

https://www.tate.org.uk/art/art-terms/m/minimalism


# artworks

https://www.wikiart.org

https://artsandculture.google.com/


### 구글코랩 실습 예제 

AI 시대 관련 기사 :  https://gist.github.com/leeseomin/a7950e4942e8f298315a484936077c07

MIT 딥러닝 코스  :  https://www.youtube.com/watch?v=njKP3FqW3Sk&list=PLHkKmgGGVneX2BzZVYGqcWbFw_7ymcZqv


선형회귀 :  https://colab.research.google.com/drive/1gH61udtFsGoB0HUmruD8TcDIYHk0mMt_?usp=sharing

딥러닝 뉴럴네트워크 기본 : https://colab.research.google.com/drive/1b8a-4M-P6c2SS3J5FCcyBWdgMo6o3sKW?usp=sharing

GAN 설명 : https://pytorch.org/tutorials/beginner/dcgan_faces_tutorial.html

MNIST GAN  설명 : https://medium.com/intel-student-ambassadors/mnist-gan-detailed-step-by-step-explanation-implementation-in-code-ecc93b22dc60

MNIST GAN 테스팅코드 : https://colab.research.google.com/drive/1Un86gDoTuWivNa2Ft0CwX-VX-s0WW69q?usp=sharing


슈퍼 해상도 esrgan  :https://colab.research.google.com/drive/1V7xwDyx8ZD9_2SgCEnmqqa5NYdzpt7Ls?usp=sharing

뉴럴스타일 :  https://colab.research.google.com/drive/1B1T3R5m8Ll8dKvdwbIAZwaUPoBuFmigh?usp=sharing

스타일갠 설명 :  https://jonathan-hui.medium.com/gan-stylegan-stylegan2-479bdf256299  ,  https://arxiv.org/pdf/1812.04948.pdf

스타일갠2 ada 추상미술  : https://towardsdatascience.com/creating-abstract-art-with-stylegan2-ada-ea3676396ffb



### dd 복사:  https://gist.github.com/leeseomin/fc1f8eb40d89d6da42579821d9814a47



### image to apng or webp 

```
ffmpeg -framerate 1 -pattern_type glob -i '*.png' \
  -c:v libx264 out.mp4
  
  
ffmpeg -i out.mp4 -plays 0  apngout.apng

ffmpeg -i  out.mp4 -vcodec libwebp -filter:v fps=fps=20 -lossless 1 -loop 0 -preset default -an -vsync 0 output.webp  

```


### 이미지 넘버링 rename  숫자로
```
a=1000
for i in *.*; do
  new=$(printf "%0d.png" "$a") #04 pad to length of 4
  mv -i -- "$i" "$new"
  let a=a+1
done
```


###  nft art generator 
https://github.com/leeseomin/nft-art-generator
