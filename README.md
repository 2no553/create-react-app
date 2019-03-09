## Version
```
- Docker version 18.09.2
- docker-compose version 1.23.2
- node v10.15.2
- npm 6.4.1
- yarn 1.13.0
- react v16.8.3
```

## Directory
```
.
├── README.md
├── docker
│   └── node
├── docker-compose.yml
└── my-app
    ├── README.md
    ├── node_modules
    ├── package.json
    ├── public
    ├── src
    └── yarn.lock
```

### Start
```
git clone https://github.com/2no553/react_docker.git
cd react_docker/
docker-compose up -d --build
```

#### Create app
```
docker-compose run --rm app npx create-react-app my-app
```

### build
```
docker-compose exec app sh
/srv/my-app # npm install
/srv/my-app # npm start
http://192.168.XX.XXX:3000/
```

### Reference
- [node \- Docker Hub](https://hub.docker.com/_/node/)
- [facebook/create\-react\-app: Set up a modern web app by running one command\.](https://github.com/facebook/create-react-app)
- [docker\-composeでコンテナが起動しない – inamuu\.com](https://inamuu.com/docker-compose%E3%81%A7%E3%82%B3%E3%83%B3%E3%83%86%E3%83%8A%E3%81%8C%E8%B5%B7%E5%8B%95%E3%81%97%E3%81%AA%E3%81%84/)
- [Docker と node\_modules と Volume Trick \- Memento memo\.](https://shotat.hateblo.jp/entry/2016/12/01/221631)
- [Quickstart: Compose and Rails \| Docker Documentation](https://docs.docker.com/compose/rails/)
- [Continuous Deployment \| Netlify](https://www.netlify.com/docs/continuous-deployment/#build-settings)
