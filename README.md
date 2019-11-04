# react-aws-todo

## Reference 
  https://www.linkedin.com/learning/aws-and-react-creating-full-stack-apps/
## Create app
```
  npx create-react-app .
```

## Amplify
Install amplify CLI
```
  sudo npm i -g @aws-amplify/cli
```
Create a user and setup the amplify
```
  amplify configure
```

```
  amplify init
  amplify add hosting 
  amplify publish
```


## Auth
```
  amplify add auth
  amplify push
```

```
  npm add aws-amplify aws-amplify-react
```

Add aws auth to project
```
import Auth from 'aws-amplify'
import awsconfig from './aws-exports'
import {withAuthenticator} from 'aws-amplify-react'

Auth.configure(awsconfig)

function App() {
 
}

export default withAuthenticator(App);
```