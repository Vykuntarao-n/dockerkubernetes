# npx Create React App Generation
As of npm@5.2.0 we can now avoid this global install and instead use npx to generate the app on the fly to get the most current libraries and avoid many dependency conflicts. This is now the recommended way to generate an app with Create React App.

1. Instead of this:
```
npm install -g create-react-app
create-react-app client
```

2. Just do this:
```
npx create-react-app client
```

Official docs on CRA usage with npx are available here:

https://create-react-app.dev/docs/getting-started#quick-start



# Basic React Commands

  ```
  npm start
  ```
  
  Starts the development server.

  ```
  npm run build
  ```
  Bundles the app into static files for production.

  ```
  npm test
  ```
  Starts the test runner.

  ```
  npm run eject
  ```
  Removes this tool and copies build dependencies, configuration files  and scripts into the app directory. If you do this, you can’t go back!

We suggest that you begin by typing:

  ```
  cd client
  npm start
  ```
  
# Start the prodution grade React applictaion 

  Build the image with the Multi stage Docker file
  ```
  docker build . -t vykuntarao1/reactfrontendapp
  ```
  
  To start the Contaier
  ```
  docker run -p 8080:80 -d vykuntarao1/reactfrontendapp
  ```
  

  
