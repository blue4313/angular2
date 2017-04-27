# angular2
Angular2 Study

# wikibook ng2 book github
https://github.com/wikibook/ng2-book

# nvm - npm version management tool
https://github.com/coreybutler/nvm-windows

# nvm download path
https://github.com/coreybutler/nvm-windows/releases

# nvm installed path
C:\Users\Administrator\AppData\Roaming\nvm

# npm installed path
C:\Users\Administrator\AppData\Roaming\npm

# nodist - npm version management tool
https://github.com/marcelklehr/nodist

# nave - npm version management tool
https://github.com/isaacs/nave

# nodejs url
https://nodejs.org/ko/

#Angular2 Setup a local development environment

	- angular2를 개발하려면 nodejs와 npm를 설치해야 한다.
	- nodejs를 설치하면 자동으로 npm도 설치된다.
	- node 버전관리를 위해 nvm, nodist, nave 등 같은 툴을 이용한다.
	* 반드시 버전을 확인하고 설치해야 함.. 버전을 다르면 작동이 안될 수도 있음...

1 . 기본설치

	1) nvm 등 버전관리 툴 없이 그냥 노드만 설치할 경우
		- https://nodejs.org/ko/ 최신버전 다운로드 해서 설치 (LTS 버전 )
		- nodejs install

	2)  nvm 등 버전관리 툴을 이용해서 설치할경우 (2개이상의 노드버전 설치가 가능, 버전별로 프로젝트 관리가 가능)
		- 기존에 설치된 nodejs를 삭제 (폴더까지 찾아서 삭제 : C:\Users\Administrator\AppData\Roaming\npm)
		- nvm install
		- cmd 실행
		> nvm install 6.10.2 (노드버전) : nvm 명령으로 노드 설치

	3) angular-cli 설치 (필수아님) (설치하면 편리하고  ng 명령을 사용할 수 있음)
		- node 6.10.2 이전 버전에서는 npm install -g angular-cli 로 설치
		- node 6.10.2 이후 버전에서는 npm install -g @angular/cli 로 설치

4) 설치확인

	- cmd 실행
	> nvm version : nvm 버전확인
	> nvm list : 설치된 노드 리스트
	> nvm use 6.10.2 (노드버전) : 사용 할 노드버전 선택 
	> node -v : 노드 버전확인
	> npm -v : npm 버전확인
	> ng -v : angular-cli 버전확인

2. 기본폴더생성

	* angular를 실행하려면 기본적으로 필요한 파일들이 있음

	- 직접 타이핑해서 만들수도 있지만, 다운로드 받거나, ng 명령어로 생성할 수 있음

	* 다운로드 받는 방법

		- Angular 사이트 (https://angular.io/) 에서 직접 다운로드

		- git 명령을 통해서 다운로드 (git 이 설치되어 있어야 함 https://git-scm.com/)
		- cmd 실행
		> git clone https://github.com/angular/quickstart.git quickstart

		- github 사이트에서 다운로드 
			https://github.com/angular/quickstart

		-  angular-cli 를 이용하는 방법
			- cmd 실행 ( angular-cli가 설치되어 있어야 함)
			> ng new project (프로젝트명) : ng new 명령으로 생성할 수 있음

	- 다운받는 파일을 압축을 풀거나 작업폴더로 이동한다.
		- cmd 실행
		> npm install : node_modules를 내려받는다. (package.json을 기반으로 필요한 모듈을 내려받고 설치함)
		> npm start 로 실행

	- angular-cli 경우
		- cmd 실행
	> ng new project (프로젝트명) : ng new 명령으로 생성할 수 있음, node_modules 까지 내려받음
	> ng serve 로 실행
  
