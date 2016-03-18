# Installation

See [angular quick start](https://angular.io/docs/ts/latest/quickstart.html)

We need to set up our development environment:
- install node and npm
- create an application project folder
- add a tsconfig.json to guide the TypeScript compiler
- add a typings.json that identifies missing TypeScript definition files
- add a package.json that defines the packages and scripts we need
- install the npm packages and typings files (npm install)

# build the Hello World app

add files

- app/app.component.ts

```ts
import {Component} from 'angular2/core';

@Component({
    selector: 'my-app',
    template: '<h1>Hello World</h1>'
})
export class AppComponent { }
```

- app/main.ts
```ts
import {bootstrap}    from 'angular2/platform/browser';
import {AppComponent} from './app.component';

bootstrap(AppComponent);
```

# start the app

npm start

=> this will compile type scripts in js
=> this will start the server

app is reachable at http://127.0.0.1:3000/

# Tour of Heroes


## Routing

turn AppComponent into an application shell that only handles navigation.
relocate the Heroes concerns within the current AppComponent to a separate HeroesComponent
add routing
create a new DashboardComponent
tie the Dashboard into the navigation structure.