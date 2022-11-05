# Vue 이커머스 대시보드 개발
이 프로젝트는 Vue 학습을 위한 가상 E-Commcerce 대시보드 repository입니다.

## 구현 메뉴
> 총 개발기간은 6 weeks 를 목표로 함
> decody, jinavely: 각자 전체 개발을 목표로 함
1. Sign-up (로그인)
2. Dashboard (대시보드)
3. Order (주문), Order Detail (주문 상세 모달)
4. Statistics (통계)

## 구현 기능
> 대시보드용 mock data는 js로 최초 제공 -> 차후 백엔드 Node.js + Sqlite3로 구현 
- 데이터 테이블, 차트, 셀렉트박스, 모달 등 UI kits는 Vuetify 프레임워크 활용
- Vuetify 차트에서 지원하지 않는 차트는 Echarts 개발
- ~~동적~~ Search Filtering 기능
- Statistics 카테고리
    - 레이아웃 위치값 로컬 저장 기능 (Vuex)
    - 컴포넌트 drag & drop 기능
    - 일부 차트 및 컴포넌트 PNG/PDF Export
- Order 페이지 
    - 검색 기능
    - Refresh 기능
    - Excel 다운
    - 기간 검색 : *https://livelybone.github.io/vue/vue-datepicker/*
- 다국어: 국/영문
- Sign-up 페이지
    - admin / shopmaster 2단계 회원 레벨링
    - 권한별로 접근 페이지 관리 : admin - 전 페이지 접근, shopmaster - Dashboard, Orders만 접근

## Figma 기반 UI & 레이아웃 구성
- Figma 기반 레이아웃 구성. why? css로 컴포넌트 구성하기 빠르며 원격 협업이 쉬움.
- 추후 차기 사이드 프로젝트인 백엔드 Node.js와 프론트엔드 React에도 Figma로 활용 예정
- Figma 레이아웃 (Sign-up, Dashboard, Orders, Stats, Order Detail modal)
    - *https://www.figma.com/file/4DELY9OqkS2UFpqqP1ouvY/e-commerce-dashboard-(share)?node-id=0%3A1*
    - 상세한 구현 설명은 figma의 Guide 레이아웃 참고

## 기술 스택
- json-server
- vue 2.0
- vue-router
- axios
- vuetify
- vuex
- echarts (vue-echarts)
- vue-grid-layout
- swiper (vue-awesome-swiper)
- lodash
- moment
- vue-i18n
- file-saver
- vue-datepicker
- Material Design

## 프로젝트 폴더 (src 하위 폴더)
- assets: 공통 이미지, 웹 폰트
- components: 모든 페이지에서 공통으로 사용하는 common 폴더와 각 페이지 이름의 폴더를 둠
    - common: 공통 컴포넌트
    - main: 메인 페이지 컴포넌트
    - products: 상세 페이지 컴포넌트
- pages: router를 통해 랜더링되는 페이지 컴포넌트
    (api 로직이나 비즈니스 로직, vuex의 스토어 관리 컴포넌트)
    - dashboard: 메인 통합 대시보드
    - order: 주문 대시보드
    - stats: 통계 대시보드
- router: 라우터
- data: mock용 데이터 (json-server 이용)
- api: 백엔드 연동 api 메서드
- stores: vuex
- styles: 전역 css
- utils: 필터 등의 유틸리티 함수
- mixins: 믹스인
- plugins: 플러그인

## JSON Server 기동
- `json-server --watch ./src/data/mockdb.json --port 4000`
- https://github.com/typicode/json-server
- 웹에서 JSON Server 기동 https://my-json-server.typicode.com/

## 기타 사항 및 관련 링크
- 아이콘 세트는 Vuetify 기반 Material Design 활용
- Vue Echart : https://vue-echarts.dev/
- Echart 문서
    - 핸드북 : https://echarts.apache.org/handbook/en/get-started/
    - 옵션 : https://echarts.apache.org/en/option.html#title
- 대시보드 drag & drop : https://jbaysolutions.github.io/vue-grid-layout/