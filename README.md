# flow-dynamic
- [HermeSys](https://hermesys.cafe24.com/)에서 운영중인 GitHub organization 입니다.
- 물의 흐름(FLOW) 방향과 속도 데이터를 이용하여 동적으로 가시화한 결과를 웹페이지에 서비스해 드리고 있습니다.
- 해당 서비스는 무료로 진행되고 있으며, 유료서비스는 준비중에 있습니다.

 ---
 
- 보유한 유속 격자/흐름격자/수심 격자 파일을 압축하여 GitHub [DATA](https://github.com/hermesys2017/flow-dynamic/tree/main/DATA) 폴더에 업로드 해주세요.
- 데이터 작업후 아래와 같이 동적 가시화된 물의 흐름을 웹페이지에서 서비스해드립니다.
- 파일은 아래 입력 데이터 규칙에 맞게 업로드해주세요.
- 대략 10 working days 이내에 구축되어 제시됩니다.
- 업로드하신 데이터는 퍼브릭에게 오픈되고, flow map 구축 작업이 완료되면 별도의 통보없이 서비스가 시작됩니다.

- Live Demo : [청미천 흐름 동적 가시화](http://210.92.123.200/flowmap/index_osim_G2D_Sample_20240307.html)
  
  ![Screenshot](/screenshots/Cheongmicheon_Dynamic_flow_20240321_1130.gif?raw=true)

## 입력 데이터
- [G2D 플러그인](https://github.com/floodmodel/G2D)을 통해 산출된 유속 격자 및 흐름 격자(Flow Direction) 결과물을 입력 데이터로 사용할 수 있습니다. 
- 입력 데이터 좌표계(SRS) = EPSG 4326, 공간해상도(Spatial Resolution)=0.0001, Raster Format만 지원합니다.
- 유속 격자와 흐름 격자는 동적으로 가시화 하기 위한 필수 파일입니다.
  - 흐름 방향 인덱스정보를 함께 제공해야함. 예) E1 = 1, S3 = 3, W5 = 5, N7 = 7
- 수심 격자 파일은 배경맵으로 사용하기 위한 것으로 필수 파일은 아닙니다.
- 아래 3 종류의 래스터 파일을 DATA 저장소에 업로드해주시기 바랍니다.
  - 유속 격자 파일(필수) - 파일명에 "Velocity" 입력 예) G2D_Sample_Velocity_10h.out
  - 흐름 격자 파일(필수) - 파일명에 "fd" 입력       예) G2D_Sample_FD_10h.out
  - 수심 격자 파일(선택) - 파일명에 "Depth" 입력    예) G2D_Sample_Depth_10h.out
 - userABC 인 경우 아래와 같은 명명 규칙 참고
  - flow-dynamic/DATA/userABC/g2d_run_20240301_v1.zip
  - flow-dynamic/DATA/userABC/g2d_run_20240301_v2.zip
  - flow-dynamic/DATA/userABC/g2d_run_20240325.zip


