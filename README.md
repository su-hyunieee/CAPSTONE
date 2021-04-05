# CAPSTONE
라즈베리 파이에서 main.py를 작동시킨후 application를 작동해야 합니다.
위치 조정및 테스트는 CAMERA_TEST.py에서 진행하였습니다.

Colab 학습 코드
train_data.py

딥러닝 
yolov3_custom2_last.weights - 딥러닝 모델
yolov3_custom2.cfg - configure file
coco.names - names file

라즈베리파이 내  코드
main.py -  전체 control tower, server 그리고 arduino와 연동
CAMERA_TEST.py - real time detect 테스트,  좌표값 위치 맞추기 테스트

아두이노 내 코드
do_motor.ino - Serial 1 , left right motor 담당
cut_motor.ino - Serial 2, cut motor 담당

iOS Application 코드
LiveCapturingApp.zip
