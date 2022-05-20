# .gitignore
[1] .gitignore
> 특정 파일 혹은 폴더에 대해 Gitdl 버전 관리를 하지 못하도록 지정하는 것

1. .gitignore에 작성하는 목록

- 민감한 개인 정보가 담긴 파일 (전화번호, 계좌번호, 각종 비밀번호 등)
- OS에서 활용되는 파일
- IDE(통합 개발 환경) 혹은 Test editor(vscode)등에서 활용되는 파일

- - 예) pycharm -> .idea/

- 개발 언어(python) 혹은 프레임 워크(dJango)에 활용되는 파일 
- - 가상 환경 : `venv/`
- - `__pycache__/`

2. .gitignore 작성 시 주의 사항
- 반드시 이름을 .gitignore로 작성합니다. 앞의 점(.)은 숨김 파일이라는 뜻입니다
- .gitignore 파일은 .git 폴더와 동일한 위치에 생성합니다.
- 제외 하고 싶은 파일은 반드시 git add 전에 .gitignore에 작성합니다
