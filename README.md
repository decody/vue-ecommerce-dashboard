# Vue 이커머스 대시보드 개발
이 프로젝트는 Vue 학습을 위한 가상 E-Commcerce 대시보드 repository입니다.

## 대시보드 레이아웃
- figma

# 구현 메뉴
- Dashboard (대시보드)
- Order (주문)
- Statistics (통계)

## 구현 기능
1. decody, jinavely: 각자 전체 개발을 목표로 함
- 다국어: 국문, 영문
- 차트 이미지파일 (PNG) Export
- 컴포넌트는 Vuetify 프레임워크 이용
- 레이아웃 내 컴포넌트 드래그 앤 드롭 기능
- 특정 페이지 Refresh 기능
- 동적 Filtering 기능

## 프로젝트 폴더 (src 하위 폴더)
- assets: 공통 이미지, 웹 폰트
- components: 모든 페이지에서 공통으로 사용하는 common 폴더와 각 페이지 이름의 폴더를 둠
    - common: 공통 컴포넌트
    - main: 메인 페이지 컴포넌트
    - products: 상세 페이지 컴포넌트
- pages: router를 통해 랜더링되는 페이지 컴포넌트
    (api 로직이나 비즈니스 로직, vuex의 스토어 관리 컴포넌트)
    - dashboard: 메인 페이지 로직 컴포넌트
    - delivery: 상세 페이지 로직 컴포넌트
    - stats: 
- router: 라우터
- api: 백엔드 연동 api 메서드
- stores: vuex
- styles: 전역 css
- utils: 필터 등의 유틸리티 함수
- mixins: 믹스인
- plugins: 플러그인
- data: mock용 백엔드 데이터

## 기술 스택
- json-server
- vue 2.0
- vue-router
- axios
- vuex

## JSON Server 기동
- `json-server --watch ./src/data/mockdb.json --port 4000`
- https://github.com/typicode/json-server
- 웹에서 JSON Server 기동 https://my-json-server.typicode.com/