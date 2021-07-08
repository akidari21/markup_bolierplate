# UI 마크업(Sass) 스타터

* **Live reloading** <br> browser update after changes
* **Automatically optimization** entry files <br> concatenate, minify and inject output files to HTML
* **[Sass](https://sass-lang.com/) for stylesheets** <br> with [the 7-1 Pattern](https://sass-guidelin.es/#the-7-1-pattern)
* **[Webpack 4](https://webpack.js.org/)** a good configuration - module bundler
* **[Bootstrap 4](http://getbootstrap.com/)** - the most popular HTML, CSS and JS framework

#### 환경설치

1. Node.js 설치 (Y:/디지털채널 개편 프로젝트/1. 프로젝트_공통/14. 설치파일/Vue 개발환경).
2. C:/scard/dev/ 하위에 자신의 작업폴더를 생성 후, cd [폴더명] 명령으로 이동
3. 저장소에서 스타터 클론 받기 `git clone http://xxxxxxxxxxxx/ui-pub.git .`
4. 클론이 완료되면 `npm install` 명령으로 환경설치 

#### 빌드 명령어

* `npm run start` ─ 파일 저장시 assets을 포함한 변경사항을 실시간 반영하는 서버 시작.
* `npm run watch` ─ 파일의 변경사항을 감지 실시간 반영.
* `npm run build` ─ assets 하위 파일들을 포함 컴파일(최적화) 진행 후 /dist 폴더에 결과 파일을 생성.
* `npm run clean` ─ 이전 버전 빌드 /dist 폴더 제거 (사용하지 않음)

#### 폴더 구조

```shell
▼ project/
│
├──▼ src/
│  ├──▼ assets/            # template asset files
│  │  ├──► fonts/          # place template fonts files here
│  │  ├──► images/         # template images files
│  │  └──▼ styles/         # template style files
│  │     ├── [...]         # 7-1 Sass architecture folders
│  │     └── main.scss     # main Sass file that references scss source files
│  ├──▼ html/              # template HTML files
│  │  ├──▼ partials/       # partials of HTML code
│  │  │  └── [...]
│  │  ├── 404.html         # example 404 error page
│  │  └── index.html       # default index page
│  │  └── [...]
│  ├──▼ scripts/           # template javascript files
│  │  ├──► modules/        # dedicated project modules
│  │  ├──▼ vendor/         # necessary parts of frameworks and libs
│  │  │  └── [...]         # Bootstrap, jQuery, etc...
│  │  └── main.js          # main javascript file that references JS source files
│  ├── index.js            # entry point of template
│  └── [...]
├──▼ dist/                 # distribution folder with production build (don't edit*)
│  ├──► css/               # output styles
│  ├──► images/            # output images
│  ├──► js/                # output javascripts
│  ├── index.html          # homepage
│  └── [...]               # miscellaneous
├──▼ node_modules/         # Node.js packages (don't edit*)
│  └── [...]
├── .babelrc               # Babel configuration file
├── .eslintrc.js           # ESLint configuration file
├── package.json           # Node.js dependencies and scripts
├── webpack.config.js      # Webpack configuration file
├── package-lock.json      # Node.js dependencies lock file (don't edit)
└── [...]                  # other files
```

