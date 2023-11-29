# ⚡Dacon : 2023전력량 예측

## Abstract
> train, building_info를 통하여 각 건물별 8월 말의 전력사용량 예측을 진행한다.

<h2> 👪 Team </h2>

> Name : 올인

<h3> 👪 Members </h3>
<table>
  <tr>
    <td> <div align=center> 👑 </div> </td>
    <td> <div align=center>  1 </div> </td>
    <td> <div align=center>  2 </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b>김다운</b> </div> </td>
    <td> <div align=center> <b>오지우</b> </div> </td>
    <td> <div align=center> <b>최지은</b> </div> </td>
  </tr>
  <tr>
    <td> <img alt="Github" src ="" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="" width="200" height="300"/> </td>
    <td> <img alt="Github" src ="" width="200" height="300"/> </td>
  </tr>
  <tr>
    <td> <div align=center> <a href="https://github.com/Daw-ny"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/woooyen"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
    <td> <div align=center> <a href="https://github.com/gyen97"> <img alt="Github" src ="https://img.shields.io/badge/Github-181717.svg?&style=plastic&logo=Github&logoColor=white"/> </div> </td>
  </tr>
</table>

<h3> 🛑 Role & Rule </h3>

> ### Ground Rule
> - 1일 3회 제출 제한이므로 각자 3회씩 제출해보되 최종적으로 팀 결합때 57회를 넘으면 안된다.
> - 회의를 통해 각자의 역할을 정하고 다음 회의까지 진행된 상황을 공유하여 서로의 피드백을 듣고 필요한 부분은 수정하였다.
> - 휴식시에는 꼭 다같이 쉴것.


<table>
  <tr>
    <td> <div align=center> <b> 이름 </b> </div> </td>
    <td> <div align=center> <b> 역할 </b> </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 김다운 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br>
	 <b>모델링 진행 </b>(MLjar-supervised모델 구현, Catboost담당) </br>
	 <b>파생변수 생성 </b>(데이터에서 발생할 수 있는 파생변수 생성)</br>
	 <b>코드 및 데이터 정리 </b>(활용한 코드 및 데이터 정리 및 취합) </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 오지우 </b> </div> </td>
    <td> <b>EDA </b>(데이터 별 결측치 및 이상치 탐색, 분포 확인)</br> 
	 <b>모델링 진행 </b>(MLjar-supervised모델 구현, LightGBM 담당) </br>
	 <b>변수 선택 </b>(제외 변수 처리 기준 생성)</br>
	 <b>코드 및 데이터 정리 </b>(활용한 코드 및 데이터 정리 및 취합) </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 최지은 </b> </div> </td>
    <td> <b>모델링 진행 </b>(MLjar-supervised모델 구현, XGBoost 담당) </br>
	       <b>코드 및 데이터 정리 </b>(활용한 코드 및 데이터 정리 및 취합) </td>
  </tr>
</table>

<h3> 📽️ Project Intro </h3>

<table>
  <tr>
    <td> <div align=center> <b> Subject </b> </div> </td>
    <td> 주어진 데이터를 활용하여 각 빌딩의 8월 말 전력 사용량을 예측 </td>
  </tr>
  <tr>
    <td> <div align=center> <b> Processing </b> </div> </td>
    <td> 1. 데이터의 각 칼럼이 어떤 의미를 갖는지 확인하고 각 칼럼의 분포 및 결측, 이상치 존재여부 확인 </br>
         2. 활용할 수 있는 파생변수를 생각하여 AutoML모델링 적용 </br>
         3. 모델링 별로 성능을 기록한 다음 최적의 성능을 보이는 모델 찾기 </td>
  </tr>
  <tr>
    <td> <div align=center> <b> Develop Enviroment </b> </div> </td>
    <td> <tt>Tool</tt>: Jupyter Notebook</td>
  </tr>
  <tr>
    <td> <div align=center> <b> Communication Enviroment </b> </div> </td>
    <td> <tt>Notion</tt>: 프로젝트를 위한 역할분담, 아이디어 브레인 스토밍, 프로젝트 관련 회의 내용 기록 </br> 
         <tt>Zoom, Offline Meeting</tt>: 실시간 대면/비대면 회의 </td>
  </tr>
</table>

<h3> 📆 Project Procedure </h3>

>  자세한 진행 내용은 [notion](https://www.notion.so/2023-AI-f38ef99e9ec3443a942003d1188565ec?pvs=4)에서 확인하실 수 있습니다.

<h3> 📂 Project Structure </h3>

> - Code
>> - 학습할 때 사용했던 코드로 현재 사용하면서 나올 수 있는 데이터는 반영하지 않았습니다.
>>
> - Data
>> - 학습시킬때 사용하였던 train, building_info와 test파일 뿐만 아니라 제출했던 숫자가 담긴 submission들이 포함되어 있습니다.

<h3> ⚙️ Architecture </h3>
<table>
  <tr>
    <td> <div align=center> <b> 분류 </b> </div> </td>
    <td> <div align=center> <b> 내용 </b> </div> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 모델 </b> </div> </td>
    <td> <tt>MLjar-supervised</tt>, <tt>XgBoost</tt>, <tt>LigthGBM</tt>, <tt>CatBoost</tt> </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 데이터 </b> </div> </td>
    <td> 데이콘 제공 데이터 train, building_info, test </td>
  </tr>
  <tr>
    <td> <div align=center> <b> 모델 평가 및 해석 </b> </div> </td>
    <td> SMAPE를 계산하여 성능이 가장 좋은 모델을 기반으로 계속해서 fitting해나간다. </td>
  </tr>
</table>
