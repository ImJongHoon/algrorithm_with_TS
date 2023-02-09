# typescript 프로젝트 생성하기

보통 많은 툴들이 자동적으로 타입스크립트 프로젝트를 생성해주지만,
수동으로 만드는 방법을 알아둔다.

1. npm init -y
2. npm install -D typescript (-D 속성으로 typescript는 devDependecies안에 설치된다.
dependencies는 어플리케이션을 배포할 때 프로덕션에 필요한 목록들이고 devDependencies는 프로덕션이 아닌 개발 목적으로만 필요한 라이브러리 등의 목록임.)
3. tsconfig.json 파일 생성.

4. tsconfig에 "include": [] 배열 생성.
이 내부에 자바스크립트로 컴파일하고 싶은 모든 디렉터리를 넣어준다.

5. tsconfig 내부의 "compilerOptions": {
        "outDir": ""
    }
    코드에는 자바스크립트로 컴파일 된 파일들의 위치를 써준다.