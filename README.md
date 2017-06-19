# KGSH Community API Server

KGSH Community의 iOS, AOS(Android) Front-End 작업을 위한 API Server부분 입니다. 라우터에서 API Server 진입을 위한 부분만 있습니다.

## 기술 스택

KGSH Community는 Timeline을 프론트엔드에서 적극적으로 사용하기 때문에 non-blocking I/O 처리에 적합한 Node.js로 작성이 되어있으며, Express.js를 사용하고 있습니다.


- **Application and Data**
  - JavaScript
  - [nginx](https://nginx.org/en/)
  - [Node.js](https://nodejs.org/)
    - [Express.js](http://expressjs.com/)
    - [body-parser](https://github.com/expressjs/body-parser)
    - [cookie-parser](https://github.com/expressjs/cookie-parser)
    - [debug](https://www.npmjs.com/package/debug)
    - [hasha](https://www.npmjs.com/package/hasha)
    - [PUG(jade)](https://pugjs.org/api/getting-started.html)
    - [morgan](https://github.com/expressjs/morgan)
    - [express-session](https://github.com/expressjs/session)
    - [mysql](https://github.com/mysqljs/mysql)
    - [serve-favicon](https://www.npmjs.com/package/serve-favicon)
    - [multiparty](https://github.com/pillarjs/multiparty)
  - [MySQL](https://www.mysql.com/)


- **Utilities**
  - [Github](https://github.com/)


- **DevOps**
  - [Travis CI](https://travis-ci.org/)


- **Business Tools**
  - [Slack](https://slack.com/)
  - [Trello](https://trello.com/)
  - [Pivotal Tracker](https://www.pivotaltracker.com/dashboard)


## 시작하기

API Server는 Core를 종속적으로 포함하고 있습니다. 즉 Core가 없으면 동작하지 않습니다.

### Core 연결

Core를 연결하는 방법은 매우 쉽습니다. Core는 반드시 APIServer/API-Server 내부에 있어야하며 이름은 소문자여야 합니다.

````bash
$ git submodule init
$ git submodule update
````

위의 소스코드를 입력하면 Core 연결이 끝 입니다.
