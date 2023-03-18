# dev_rails_api_nuxt

- docker images
  - api
    - ruby:3.2.1
  - mysql
    - mysql:8.0

- git clone or fork

```
mkdir ~/www
cd ~/www
git clone git@github.com:tatuya4451/dev_rails_api_nuxt.git
```

- docker run

```
cd ~/www/dev_rails_api_nuxt/docker/dev/
docker-compose up -d
```

- app deploy

```
docker-compose exec api bash
bundle install
rails db:create
rails s -p 3000 -b '0.0.0.0'
```

- Access

http://localhost:3000/

![image](https://user-images.githubusercontent.com/66053927/225494641-9db4575a-afc3-452b-ba23-8e90bd679128.png)

- front build
```
docker-compose exec frontend sh
yarn install
yarn dev -o
```

- Access

http://localhost:8000/

<img width="1406" alt="スクリーンショット 2023-03-16 12 22 13" src="https://user-images.githubusercontent.com/74761742/225505548-1fa877e2-38ff-4587-97b3-79826a8c0583.png">


- DB login

```
docker-compose exec db bash
mysql -u root
```
