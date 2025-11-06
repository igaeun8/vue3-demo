# vue-demo

## Vue 3 마이그레이션 완료

이 프로젝트는 Vue 2에서 Vue 3 스타일로 전환되었습니다. 모든 컴포넌트가 Vue 3의 `defineComponent`를 사용하도록 업데이트되었으며, TypeScript 지원이 추가되었습니다.

### 주요 변경사항

#### 1. 컴포넌트 정의 방식 변경
- 모든 컴포넌트에 `defineComponent` 적용
- TypeScript 지원을 위해 `<script lang="ts">` 추가
- Vue 3 호환성을 위한 구조로 전환

#### 2. 전환된 컴포넌트 목록

**example1/**
- `E-01-instance.vue` - 기본 인스턴스 컴포넌트
- `E-02-reactive.vue` - 반응형 데이터 및 computed 속성 (오타 수정: `lasstName` → `lastName`)
- `E-03-binding.vue` - 양방향 바인딩 예제

**example2/**
- `E-04-directives.vue` - 디렉티브 사용 예제

**example3/**
- `ParentComponent.vue` - 부모-자식 컴포넌트 통신
- `ChildComponent.vue` - Props 및 이벤트 emit

**example4/**
- `ParentComponent.vue` - Provide/Inject 패턴
- `ChildComponent1.vue` - Inject 사용 예제
- `ChildComponent2.vue` - Inject 사용 예제

**example5/**
- `E-07-Options-API.vue` - Options API 예제 (TypeScript 타입 추가)
- `E-08-composition-api.vue` - Composition API 예제
- `E-09-composition-API2.vue` - `<script setup>` 문법 예제

**example6/**
- `E-10-ref.vue` - ref 사용 예제
- `E-11-reactive.vue` - reactive 사용 예제
- `E-12-ref-component.vue` - 컴포넌트 ref 사용 예제

#### 3. 타입 안정성 개선
- 메서드 매개변수에 TypeScript 타입 추가
- Watch 콜백 함수에 타입 지정
- 모든 컴포넌트가 TypeScript로 작성됨

#### 4. 호환성
- Vue 3.2.13 사용
- 기존 동작 및 화면 유지
- 기능 추가 없이 리팩토링만 수행

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
