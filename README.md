# vue-demo
실습 2-2. Vue2 문법을 Vue3로 전환 프로젝트입니다. 

모든 컴포넌트가 Vue 3의 `defineComponent`를 사용하도록 업데이트되었으며, TypeScript 지원이 추가되었습니다.

## 주요 변경사항

#### 1. 컴포넌트 정의 방식 변경
- 모든 컴포넌트에 `defineComponent` 적용
- TypeScript 지원을 위해 `<script lang="ts">` 추가
- Vue 3 호환성을 위한 구조로 전환

#### 2. 타입 안정성 개선
- 메서드 매개변수에 TypeScript 타입 추가
- Watch 콜백 함수에 타입 지정
- 모든 컴포넌트가 TypeScript로 작성됨

#### 3. 호환성
- Vue 3.2.13 사용
- 기존 동작 및 화면 유지
- 기능 추가 없이 리팩토링만 수행
- 
#### 4. 동작 확인용 스크린샷

**example1/**
- `E-01-instance.vue` - 기본 인스턴스 컴포넌트
<img width="360" height="143" alt="image" src="https://github.com/user-attachments/assets/49acb4f5-2b7e-43c4-931a-2004b0f486de" />

- `E-02-reactive.vue` - 반응형 데이터 및 computed 속성 (오타 수정: `lasstName` → `lastName`)
<img width="224" height="134" alt="image" src="https://github.com/user-attachments/assets/73212d9f-3c48-4cc7-9dd3-ceb4c1c935bb" />

- `E-03-binding.vue` - 양방향 바인딩 예제
<img width="364" height="152" alt="image" src="https://github.com/user-attachments/assets/a360aa84-2778-4144-a995-3ece5980009e" />

**example2/**
- `E-04-directives.vue` - 디렉티브 사용 예제
<img width="359" height="391" alt="image" src="https://github.com/user-attachments/assets/b2ca6d64-d94a-4913-b461-564bda6e758d" />

**example3/**
- `ParentComponent.vue` - 부모-자식 컴포넌트 통신
- `ChildComponent.vue` - Props 및 이벤트 emit
<img width="281" height="169" alt="image" src="https://github.com/user-attachments/assets/2e68feeb-388d-48ef-8cf2-d97e1db8f233" />

**example4/**
- `ParentComponent.vue` - Provide/Inject 패턴
- `ChildComponent1.vue` - Inject 사용 예제
- `ChildComponent2.vue` - Inject 사용 예제
<img width="212" height="126" alt="image" src="https://github.com/user-attachments/assets/f2869011-abdf-4a4c-90af-a00963f113ec" />

**example5/**
- `E-07-Options-API.vue` - Options API 예제 (TypeScript 타입 추가)
- `E-08-composition-api.vue` - Composition API 예제
- `E-09-composition-API2.vue` - `<script setup>` 문법 예제
<img width="405" height="173" alt="image" src="https://github.com/user-attachments/assets/b83b4184-69bd-4b7f-8291-1b71e8f20e88" />

**example6/**
- `E-10-ref.vue` - ref 사용 예제
<img width="232" height="111" alt="image" src="https://github.com/user-attachments/assets/c9feab39-e421-4aff-a9cf-1a697167fa3e" />

- `E-11-reactive.vue` - reactive 사용 예제
<img width="186" height="128" alt="image" src="https://github.com/user-attachments/assets/5a4538bb-69bf-44d1-bef3-7e21e7341c9d" />

- `E-12-ref-component.vue` - 컴포넌트 ref 사용 예제
<img width="262" height="59" alt="image" src="https://github.com/user-attachments/assets/e471275b-5fd1-4b92-be27-7a5a8ddc5883" />



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
