This tutorial uses react along with typescript to build this project. React is a popular javascript framework that allows interactive apps to be built easily. Typescript is a modified form of javascript that provides type safety to javascript so user does not encounter any variable type errors during execution.

In the first step we use boilerplate code to start. Press Ctrl + ~ to open terminal in the folder where you want to base your project. Running the following command:
```console
    yarn create react-app whatsapp-clone-client --template typescript
```

creates a new folder called `whatsapp-clone-client` inside present working directory. This uses yarn which is a package manager built for javascript/typescript.

The folder has been named client cause our app will be split into two part. The client side handles the front-end and renders the app to show the content to the user. Afterwards a server side will be created to handle the back-end and link to the front-end to deliver the content needed to be displayed.

### Reviewing created template:
After running the `yarn create react-app` command, you can see the directory created has been populated with folders and sample files inside which can be run to view the sample react program. Now we can move present working directory inside the folder in order to use commands that directly only the contents inside the folder as well as allow the command line to run commands that can only be run in the root directory. Once the command has been successfully completed you can move the present working directory inside the folder with the following command:
```console
    cd whatsapp-clone-client
```
These files populated when run will view a sample react app. To view this simply run:
``` console
    yarn start
```
This will run the code and serve a webpage on your computer on port 3000. If webpage does not automatically open simply click open [http://localhost:3000](http://localhost:3000) in your web browser. The welcoming page will be shown similar to the one below.