# svelte-overview

## Quick Start Guide
+ Svelte 공식 문서에서 Svelte 프로젝트를 빠르게 만들 수 있는 2가지 방법(REPL과 digit)을 이야기합니다. 
+ REPL, digit으로 프로젝트를 만들수 있는 방법을 이야기하도록 하겠습니다. 자세한 내용은 quickstart guide를 참고 바랍니다.
  
### REPL 사용
+ REPL(Real Eval Print Loop)이란 사용자의 입력을 받아 실행하고 결과를 사용자에게 보여주는 프로그래밍 환경을 말합니다.
+  CDN으로 Svelte를 사용할 수 없어서 CodePen 등의 웹 IDE를 사용할 수 없습니다. 
+  Svelte는 이런 단점을 보완하기 위해 자체적으로 REPL을 제공하는 것으로 보입니다.
+  Svelte는 빌드 타임에 반응형이 결정됩니다
+  이런 특징은 런타임 동안에 변경사항을 찾아야 하는 오버헤드를 줄여 속도를 개선하는 장점이 있지만, CDN 등으로 Svelte를 사용할 수 없는 단점도 있습니다.
  
+ Svelte REPL에서 코딩한 후 코딩한 프로젝트를 다운로드할 수 있습니다
+ svelte-app.zip으로 다운로드되는데, 파일의 압축을 풀고 아래와 같이 프로젝트를 실행할 수 있습니다.
  ```
    cd /path/to/svelte-app
    npm install
    npm run dev

+ 이 방법을 사용하면 rollup 번들러(bundler)를 사용한 프로젝트가 만들어집니다.


### digit 사용
+ digit를 사용하여 프로젝트를 만들 수 있습니다. 
+ Svelte는 template와 template-webpack 두 가지 템플릿 프로젝트를 제공합니다.


#### template
+ sveltejs/template은 rollup 번들러를 사용하는 템플릿입니다. 
+ 템플릿을 다운로드 하는 방법은,
```
npx degit sveltejs/template my-svelte-project
## or download and extract this .zip file
cd my-svelte-project

npm install
npm run dev
```

+ 위의 코드와 같이 rollup 번들러를 사용하는 템플릿을 다운로드할 수 있습니다.
+ 이 방법을 사용하면 sveltejs/template에 올라와 있는 프로젝트가 만들어집니다.

#### webpack template
+ sveltejs/template-webpack은 webpack을 사용하는 템플릿입니다. 템플릿을 다운로드하는 방법은,
```
npx degit sveltejs/template-webpack my-svelte-project
## or download and extract this .zip file
cd my-svelte-project

npm install
npm run dev
```

#### 프로젝트 구성 커스터마이징
+ sveltejs/template(혹은 sveltejs/template-webpack)의 깃허브(github) 레파지토리(repository)를 포크(fork) 하여 커스터마이징 한다면,
```
npx degit your-name/template my-new-project
```
+ 위의 코드로 커스터마이징한 프로젝트 구성으로 손 쉽게 프로젝트를 만들 수 있습니다.