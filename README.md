README
================

Build
----------------

```bash
$ docker build -t 'koduki/dev-rails' .
```

Create project
----------------

```bash
$ docker run -it -p 3000:3000 -v `pwd`:/usr/src/app -w /usr/src/app koduki/dev-rails bundle install
$ docker run -it -p 3000:3000 -v `pwd`:/usr/src/app -w /usr/src/app koduki/dev-rails rails new .
```