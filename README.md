인하대학교 2020년2학기 컴퓨터공학종합설계 ! !
WELLRE = Well + Recycle 
라즈베리 파이를 중심으로 애플리케이션과 아두이노가 연동되어 셋이 신호를 주고 받으며 전체 동작이 진행됩니다 ! ! 
500ml 생수병의 라벨의 유무를 판단하고 위치를 알아내어 라벨을 제거 한 후, 분류하는 기기



# CAPSTONE
라즈베리 파이에서 main.py를 작동시킨후 application를 작동해야 합니다.
위치 조정및 테스트는 CAMERA_TEST.py에서 진행하였습니다.

1.Colab 학습 코드
train_data.py -> yolov3-tiny custom해서 colab에서 학습시켰습니다
              -> 이거 구글링해도 잘 안나와서 힘들었는데 다들 보고 하시면 좋겠습니다

2.딥러닝 
yolov3_custom2_last.weights - 딥러닝 모델, 1번 코드로 학습시킨 결과물
yolov3_custom2.cfg - configure file - batch랑 filter class 설정하는 부분
coco.names - names file  - pet, label로 구분하였습니다. 검출하고자 하는 목록

3.라즈베리파이 내  코드
main.py -  전체 control tower, server 그리고 arduino와 연동
CAMERA_TEST.py - real time detect 테스트,  좌표값 위치 맞추기 테스트

4. 아두이노 내 코드
do_motor.ino - Serial 1 , left right motor 담당  -> 컨베이어 벨트 움직임 담당
cut_motor.ino - Serial 2, cut motor 담당         -> 절단기 내리기

5. iOS Application 코드 
LiveCapturingApp.zip -> WellRe 애플리케이션 코드 (성주 담당)
