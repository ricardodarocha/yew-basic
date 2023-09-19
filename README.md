# RealWorld Example App

See the tutorial
https://www.youtube.com/watch?v=KmOeFrwz8BM

> ### axum + yew + shuttle codebase containing real world examples (CRUD, auth, advanced patterns, etc) that adheres to the [RealWorld](https://github.com/gothinkster/realworld) spec and API.


### [Demo](https://realworld-axum-yew-shuttle.shuttleapp.rs/)&nbsp;&nbsp;&nbsp;&nbsp;[RealWorld](https://github.com/gothinkster/realworld)


This codebase was created to demonstrate a fully fledged fullstack application built with **axum + yew + shuttle** including CRUD operations, authentication, routing, pagination, and more.

We've gone to great lengths to adhere to the **axum + yew + shuttle** community styleguides & best practices.

For more information on how to this works with other frontends/backends, head over to the [RealWorld](https://github.com/gothinkster/realworld) repo.


# How it works

Just clone it and run wasmsetup.bat  (if you using windows) and then cargo install and trunk serve --port 9292 --open

# Getting started

## Compile frontend

First, install [trunk](https://trunkrs.dev/)

```sh
$ cargo install --locked trunk
```

And then, compile using trunk.

```sh
$ cd frontend
$ trunk build --release
```

Copy `dist` directory to backend directory.

```sh
$ cp -r dist ../backend
```

## Compile backend

First, install `cargo-shuttle`

```sh
$ cargo install cargo-shuttle
```

To run locally:

```sh
$ cd backend
$ cargo shuttle run
```

To deploy to shuttle server:

```sh
$ cd backend
$ cargo shuttle project new --name {name-of-app}
$ cargo shuttle deploy
```

