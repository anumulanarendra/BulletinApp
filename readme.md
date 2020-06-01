# React Bulletin board with Clean architecture
### Outline
Please build a single page Bulletin board application that lets users Post and add comments.

#### Features
  
* User login page with id and password(Should allow any userid and password and Not required any validations,test users).
* Board page with list of posts and Add Post form
* Optional stretch goal: Add Comments Form 

#### Notes

* You can use libraries and frameworks as you see fit.
* You can use starter projects such as create-react-app.
* Commit all changes to a Git repository and follow good commit message practice.
* Don't spend more than a couple of hours. The goal is to show how you work, not to deliver production-ready code.
* Focus on good application structure, not a working but hacky solution.
* Styles aren't important but your solution needs to work on mobile and desktop.
* Make sure there's a README with instructions on how to get started.
* When you're done, send us a link to the Git repo.


## Use Stack
Typescript, Webpack, React, Redux, Jest, Enzyme

## Clean Architecture
![Alt Clean architecture](/readme/clean-architecture.png)
As with many architectures, the primary purpose of a clean architecture is to separate concerns. Divide the hierarchy according to each interest, design domain-centric rather than detailed implementation, and make sure that the internal area does not depend on external elements such as the framework or database UI.
  
* Distinguish between detailed implementation areas and domain areas.
* The architecture is not framework dependent.
* The outer zone depends on the inner zone, the inner zone does not depend on the outer zone.
* Both high-level and low-level modules rely on abstraction.


## Communitaction Flow
![Alt Communitaction Flow](/readme/communication-flow-v4.png)
In simple diagram, it is as above.

## Directory Structure
```
./src
├─ adapters
│  ├─ presenters
│  ├─ repositories
│  └─ infrastructures
├─ domains
│  ├─ aggregates
│  ├─ entities
│  ├─ useCases
│  └─ valueObjects
├─ frameworks
│  └─ web
│     ├─ components
│     │  ├─ atoms
│     │  ├─ molecules
│     │  ├─ organisms
│     │  ├─ templates
│     │  └─ pages
│     ├─ redux
│     │  ├─ reducer
│     │  └─ store
│     └─ viewModels
└─ interfaces
   ├─ entites
   ├─ frameworks
   ├─ infrastructures
   ├─ repositories
   ├─ useCases
   ├─ viewModels
   └─ valueObjects
```

* The default directory is organized based on layers of clean architecture. [frameworks / adapters / domains(useCases / entities)]
* For component directory , refer to [[ Atomic Design](https://bradfrost.com/blog/post/atomic-web-design/#atoms)]. [atoms / molecules / organisms / templates / pages]


## Application Running
#### Install
```
$ npm install
```
#### Start
```
$ npm start
```
#### Test
```
$ npm test
```


## Roadmap
- [x] Board sample implementation
- [x] Read me writing
- [x] Style component
- [x]Creating test cases
- [] Implementation of test users with back-end server
