# flow-dynamic
- [HermeSys](https://hermesys.cafe24.com/)에서 운영중인 GitHub organization 입니다.
- 물의 흐름(FLOW) 방향과 속도 데이터를 이용하여 동적으로 가시화 할 수 있습니다.
- 해당 서비스는 무료로 진행되고 있으며, 유료서비스는 준비중에 있습니다.

 ---
 

- 보유하신 유속 격자/흐름격자/수심 격자 파일을 GitHub [DATA](https://github.com/hermesys2017/flow-dynamic/tree/main/DATA) 폴더에 업로드해주시면, 아래와 같이 동적 가시화된 물의 흐름을 보실 수 있습니다.

  - Live Demo : [청미천 흐름 동적 가시화](http://210.92.123.200/flowmap/index_osim_G2D_Sample_20240307.html)
  
  ![Screenshot](/screenshots/Cheongmicheon_Dynamic_flow_20240321_1130.gif?raw=true)

## 입력 데이터
- G2D 플러그인을 통해 산출된 유속 격자 및 흐름 격자 결과물을 입력 데이터로 사용할 수 있습니다. 
- 입력 데이터 좌표계는 EPSG 4326, 해상도 0.0001 이어야하고, 래스터 포맷만 가능합니다.
- 유속 격자와 흐름 격자는 동적으로 가시화 하기 위한 필수 파일입니다.
- 수심 격자 파일은 배경맵으로 사용하기 위한 것으로 필수 파일은 아닙니다.
- 아래 3 종류의 래스터 파일을 DATA 저장소에 업로드해주시기 바랍니다.
  - 유속 격자 파일(필수) 예) 01_G2D_Sample_fdTest_Velocity_10_00h.out
  - 흐름 격자 파일(필수) 예) 01_G2D_Sample_fdTest_FDmaxVelocity_10_00h.out
  - 수심 격자 파일(선택) 예) 01_G2D_Sample_fdTest_Depth_10_00h.out

