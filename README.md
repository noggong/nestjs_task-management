# nestjs_task-management

# CLI설치
$ npm install -g @nestjs/cli

# App 생성


============= Module ================
- 최소 한개의 모듈을 가지고 있으며 (root module), 그 모듈은 앱이 실행될때 실행된다
- 모듈은 기능별로 컴포넌트를 구성할수 있는 효과적인 방법이다
- module은 싱글톤이며, 따라서 다른 여러 모듈에서 import 가능하다
- dacorator는 nestjs 앱의 구조를 조직하는 것에 사용되어지는 metadata를 지원한다.
- dacorator: @Module
=====================================

============== @Module ===============
- providers: 프로바이더 배열 DI
- controllers: 모듈 내부에 인스턴스가 될 컨트롤러 배열
- exports: 다른 모듈에 export 될 프로바이더 배열
- imports: 해당 모듈에 필수 조건 모듈 리스트. export 된 프로바이더들이 해당 모듈에서 DI를 통해 사용되어지도록한다
======================================


task 모듈 생성

$ yarn nest g module tasks


============== Controller =============
- request / response 핸들링을 관장한다.
- 특정한 path에 연결된다 (ex: /tasks)
- endpoint handler를 포함한다. (GET, POST, DELETE)
- 같은 모듈내에서 프로바이더 의존정 주입하고 사용할수 있다.
- dacorator : @Controller
=======================================
