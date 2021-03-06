### [사용법]  

<br></br>**HCI를 사용하기 전에 TM5도 사용하실 것을 권장합니다. 또한 테스트 툴은 모두 예방 차원에서 돌리는 것이므로 너무 지나치게 큰 신뢰를 가지시면 안됩니다. 또한 실사용 시 GPU를 통해 램에 가해지는 열기도 생각하셔야합니다!**<br></br> <br></br>

1. https://github.com/bumju08/EasyHCI/releases 에 접속하여 가장 최신 글  Assets 구역 내의 최상단 zip 파일을 다운받습니다.  
![down1](https://user-images.githubusercontent.com/74810045/115340728-3479a400-a1e2-11eb-9c3f-a2e036ee5974.png)  <br></br><br></br>
2. 한 폴더에 모든 파일을 압축해제 해줍니다.  <br></br>

3. EasyHCI 실행     
![1](https://user-images.githubusercontent.com/74810045/115333182-3177b700-a1d4-11eb-90a2-a1da2f3066e0.png)   <br></br> <br></br>

4. 예 누르기 (**프로세스가 모두 종료되므로 중요한 작업을 하고 있었다면 꼭 저장해주세요. 책임지지 않습니다.** 예외처리가 가능하며, 아니오를 누르시면 어떤 프로세스도 종료되지 않습니다. **보통 테스트하기 전에 클리너를 통해 프로세스 정리부터 하셔서, 따로 프로그램 사용할 필요 없이 편하게 하시라고 넣은 기능입니다.**)  
![2](https://user-images.githubusercontent.com/74810045/115333184-32104d80-a1d4-11eb-8729-d1924ec36166.png)   <br></br> <br></br>
  
5. 이후 메모리 점유율이 95% 이상으로 상승하며 통과율이 0%에서 서서히 증가될 것입니다. 테스트가 정상 시작되었습니다.  
![3](https://user-images.githubusercontent.com/74810045/115333187-32a8e400-a1d4-11eb-8f77-4ccd4f8a389d.png)   <br></br> <br></br>
  
6. 테스트가 정상시작되었으면 설정 탭을 누르신 뒤 최상단 **목표치**의 값을 원하는 수치로 조정해주세요. 400%인 경우 400%까지만 테스트합니다. 보통 **800%에서 1400% 사이**로 많이들 테스트하시며, 과하게는 2000%에서 3000%까지 테스트하시는 분들도 있습니다. 한번 수치를 조정하시면 그 다음부터 설정 값은 PC에 저장됩니다.<br></br>**저장 경로**: 프로그램 경로 > Resources > Settings.txt  
![4](https://user-images.githubusercontent.com/74810045/115333192-33417a80-a1d4-11eb-92c2-9eb48a0642c6.png)   <br></br> <br></br>
  
7. 여러가지 도움되는 설정들이 있으니 입맛대로 설정해보셔요. <br></br>**테스트 - 수동/자동** 기능을 통해 실행될 HCI Memtest 프로세스의 개수와, 각 프로세스가 테스트할 메모리 크기를 조절할 수 있습니다. 다만, 자동으로 사용하시면 PC에 맞게 알아서 설정해주니 **따로 설정해주실 필요는 없습니다.**<br></br>**스크린샷** 은 프로그램이 특정 조건이 성립될 때 자동으로 스크린샷을 찍게 해주는 기능입니다. **HCI Screenshots** 폴더에 저장됩니다.<br></br>**소리 알림** 은 오류가 발생하거나, 테스트가 성공한 이후 소리를 통해 알려줍니다. PC에 스피커를 연결하셔서 볼륨을 크게 해놓으시면 다른 일을 하다가도 금방 알아차릴 수 있겠죠?<br></br>**마지막 행동** 은 오류가 발생하거나, 테스트가 성공한 이후 어떤 행동을 할지 결정하는 항목입니다. **PC 종료** 로 설정하신 경우 테스트가 끝나자마자 로그 작성/스크린샷을 한 뒤 PC가 종료됩니다. 테스트가 끝난 이후 EasyHCI Log.txt 파일을 열어보시거나, HCI Screenshots 폴더의 스크린샷들을 살펴보셔서 테스트 결과를 확인할 수 있습니다. PC의 안정성이 매우 낮아 테스트 도중에 블루스크린이 뜨거나 PC가 다운되어버리면 로그와 스크린샷이 남지 않으므로, 프로그램 돌려놓고 외출하시더라도 최소 10~20분정도는 제대로 돌아가는 것을 확인해보시고 외출하시길 권장드립니다.<br></br>**기타 - 프로그램이 켜질 때 즉시 테스트** 를 체크해제 해주시면 프로그램이 켜지고 직접 테스트 시작 버튼을 누르셔야 테스트가 진행됩니다.<br></br>
![5](https://user-images.githubusercontent.com/74810045/115333195-3472a780-a1d4-11eb-8ba9-c3e3dc9fffae.png)   <br></br> <br></br><br></br><br></br>
  
  
  
  

  

  
  
### [프로세스 예외처리 방법]  
1. Resources 폴더에 들어가줍니다.  
![ex1](https://user-images.githubusercontent.com/74810045/115333792-3d17ad80-a1d5-11eb-93f3-46674aa803cb.png)   <br></br> <br></br>
  
2. mcExcept.txt 파일을 열어줍니다.  
![ex2](https://user-images.githubusercontent.com/74810045/115333793-3d17ad80-a1d5-11eb-806b-c751ad5b18f2.png)   <br></br> <br></br>
  
3. 파일에 설명되어있는대로, 대소문자 구별 없이 확장자는 제외하셔서 프로세스명을 적으시면 됩니다. 끝!  
![ex3](https://user-images.githubusercontent.com/74810045/115333796-3e48da80-a1d5-11eb-8eb6-f644c90d479b.png)   <br></br> <br></br>
  
4. 만약 컴맹이라 잘 모르시겠으면 아래 예시를 참고하세요. Ctrl+Shift+ESC를 누르셔서 작업 관리자를 열어주세요.  
   카카오톡을 예외처리해보겠습니다. 카카오톡 프로세스를 찾아 우클릭 해주신 뒤, "세부 정보로 이동"을 눌러주세요.
![ex4](https://user-images.githubusercontent.com/74810045/115333798-3e48da80-a1d5-11eb-88b8-d76bfafdf3c3.png)   <br></br> <br></br>
  
5. 그럼 아래와 같이 카카오톡 프로세스명 + 확장자명이 나옵니다. (KakaoTalk.exe)  
   여기서 확장자인 .exe 부분은 제외하고 KakaoTalk만 외워주세요.  
![ex5](https://user-images.githubusercontent.com/74810045/115333801-3ee17100-a1d5-11eb-9b55-8b97e533a542.png)   <br></br> <br></br>
  
6. 아까 열어두었던 mcExcept.txt 파일의 최하단에 외워두셨던 KakaoTalk을 그대로 입력해주세요. 대소문자는 구분하지 않으셔도 됩니다.  
   이후 파일을 그대로 저장해주시면 끝입니다.
   <br></br>**윈도우 기본 프로세스/EasyHCI는 적지 않으셔도 자동 예외처리되며, HWInfo/ZenTimings/Aida64는 1.0.7버전 첨부파일에 기본적으로 예외처리되어 있습니다.**  
![ex6](https://user-images.githubusercontent.com/74810045/115333802-3f7a0780-a1d5-11eb-9289-5ae39eda6532.png)   <br></br>
  
  
