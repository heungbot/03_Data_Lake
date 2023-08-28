# 03 Config Data Lake by using Lake Formation and Glue

## [ 01 프로젝트 설명 ]
프로젝트 명 : Lake Formation을 이용한 권한 세분화 데이터 레이크 구축

프로젝트 인원 : 1명

프로젝트 기간 : 2023.08 ~ 

프로젝트 소개 : 
이 프로젝트는 가상의 회사가 현재 운영 중인 데이터베이스(DB), 서버 및 서비스를 운영중임을 전제로 하며 다양한 방법을 통해 수집한 데이터를 S3 버킷에 저장한 후, Lake Formation을 활용하여 세분화된 권한을 가진 데이터 레이크를 구축하는 데 초점을 두고 있습니다.
더불어, AWS Glue의 Crawler와 Catalog 기능을 활용하여 데이터를 관리하고 기초적인 ETL(Job)을 수행함으로써 데이터를 요구사항에 맞게  공할 수 있다는 것을 보여주며, Athena를 이용하여 간단한 쿼리 실행하는 프로젝트입니다.

***

## [ 02 클라이언트 상황 ]

* IDC 중 일부를 임대하여, 자사와 먼 거리에 6대 이상 운영중

* AWS RDS, S3 등의 서비스를 이미 운영하고 있음.

* 회사가 성장함에 따라 수집되는 데이터의 증가

* 기간 한정 할인 이벤트 및, 다양한 새로운 서비스 런칭을 계획하고 있음.

* 추 후 사내 데이터를 이용하여 대규모 머신러닝을 진행할 예정

***

## [ 03 요구사항 ]

* 온프레미스, 클라우드에 존재하는 데이터를 하나의 스토리지에 저장

* 데이터 관리 및 사내 요구사항에 부합하기 위해 각 ETL 과정의 결과물을 s3에 저장

* 확장성 및 탄력성 확보 및 데이터 사용에 대한 모니터링 요망

* 사내 각 팀에게 조건에 맞는 필요 데이터만 접근할 수 있도록 세분화된 엑세스 권한 부여 요망

***

## [ 04 다이어 그램 ] 
<img width="1401" alt="DataLake_diagram" src="https://github.com/heungbot/03_Building_Data_Lake_Using_Lake_Formation/assets/97264115/4a2ee15c-0245-49ab-883b-f26d9326ac83">
