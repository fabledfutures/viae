# Welcome to VIAE!

This is our custom fork of [Pocketbase](https://github.com/pocketbase/pocketbase). We are customizing and extending Pocketbase to better fit our needs. 
We do not build binaries of this repo. If you are looking for an off-the-shelf backend as a service, go check out [Pocketbase](https://github.com/pocketbase/pocketbase). 
Be sure to show [Gani Georgiev](https://github.com/ganigeorgiev) some love for the AMAZING work he has done!

**While [Pocketbase](https://github.com/pocketbase/pocketbase) is still pre-v1, most of our changes are minimal. We have planned changes that we will start to impliment once [Pocketbase](https://github.com/pocketbase/pocketbase) is in a stable v1.**


While [Pocketbase](https://github.com/pocketbase/pocketbase) is intended to be an entire backend solution, VIAE is intended to just be the API layer of the backend, providing primarily CRUD, AUTH, and RPC. (https://github.com/pocketbase/pocketbase) team. 

VIAE differs from [Pocketbase](https://github.com/pocketbase/pocketbase) in the following major ways:

- VIAE is inteded to be used with a managed, scalable database like PostgreSQL. [Pocketbase](https://github.com/pocketbase/pocketbase) uses an embedded SQLite. In reality MOST simple web and mobile apps do not need more than SQLite. However our applications rely heavily on the scale and analytical capabilities of systems like PostgreSQL. 
- VIAE is purely a Go framework for building custom API layers on the backend. It is not a complete solution. For apps that just need AUTH and CRUD, [Pocketbase](https://github.com/pocketbase/pocketbase) is going to be more than enough. [Pocketbase](https://github.com/pocketbase/pocketbase) already allows you to add custom routes and jobs too! We are simply configuring VIAE to be the CRUD and AUTH parts of the API layer so that we can focus on the services that go along with the API to power our applications.
- VIAE will expand the dashboard UI with more features that let application owners assess the security of their applicaiton, the nature of the usrs, and configuring caches and databases that can be deployed alongside VIAE.
- VIAE is being configured to scale out, by allowing multiple instances to be used behing a load balancer. This is only possible by moving to an external database and changing some configurations. 

**For documentation and examples of working with the API, please visit https://pocketbase.io/docs.**


> [!WARNING]
> This project is primarily being developed for our own purposes. This is not intended to be a complete package or solution for anyone to use. We also make no guarantee that we will not introduce breaking changes from time to time. 
> However, we welcome ANYONE to use this framework and power their own applications!
> We intend to adopt nearly all upstream changes in [Pocketbase](https://github.com/pocketbase/pocketbase). However our needs differ greatly from the vision of the [Pocketbase](https://github.com/pocketbase/pocketbase) maintainers. As such, some features of [Pocketbase](https://github.com/pocketbase/pocketbase) may end up working very differently in VIAE. Whenever the two roadmaps align, we are committed to pushing our changes upstream to the [Pocketbase](https://github.com/pocketbase/pocketbase) project! 

## API SDK clients

All of our changes will remain compatable with the Pocketbase front-end SDKS.

- **JavaScript - [pocketbase/js-sdk](https://github.com/pocketbase/js-sdk)** (_browser and node_)
- **Dart - [pocketbase/dart-sdk](https://github.com/pocketbase/dart-sdk)** (_web, mobile, desktop_)

## Security

If you discover a security vulnerability within VIAE, please send an e-mail to **support at fabledfutures.com**.

All reports will be promptly addressed, and you'll be credited accordingly.

## Contributing

VIAE is free and open source project licensed under the [MIT License](LICENSE.md).
You are free to do whatever you want with it.

Most contributions should be submitted as PRs to [Pocketbase](https://github.com/pocketbase/pocketbase). However, if you have a features or bug fixes that do not integrate into [Pocketbase](https://github.com/pocketbase/pocketbase)'s vision, feel free to open a PR here. Please bear in mind that we are developing this for our own purposes, and PRs will be accepted under that lense. 
