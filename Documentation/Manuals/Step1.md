# 1. Creating a basic React App

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

[Sample-Page](/Documentation/Resources/Sample_Page.png)

Now lets look at the files created automatically and how they serve the webpage shown on the browser.
The file opened by the browser is index.html that sits inside the `/public` folder.

```HTML
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />
    <meta
      name="description"
      content="Web site created using create-react-app"
    />
    <link rel="apple-touch-icon" href="%PUBLIC_URL%/logo192.png" />
    <!--
      manifest.json provides metadata used when your web app is installed on a
      user's mobile device or desktop. See https://developers.google.com/web/fundamentals/web-app-manifest/
    -->
    <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
    <!--
      Notice the use of %PUBLIC_URL% in the tags above.
      It will be replaced with the URL of the `public` folder during the build.
      Only files inside the `public` folder can be referenced from the HTML.

      Unlike "/favicon.ico" or "favicon.ico", "%PUBLIC_URL%/favicon.ico" will
      work correctly both with client-side routing and a non-root public URL.
      Learn how to configure a non-root public URL by running `npm run build`.
    -->
    <title>React App</title>
  </head>
  <body>
    <noscript>You need to enable JavaScript to run this app.</noscript>
    <div id="root"></div>
    <!--
      This HTML file is a template.
      If you open it directly in the browser, you will see an empty page.

      You can add webfonts, meta tags, or analytics to this file.
      The build step will place the bundled scripts into the <body> tag.

      To begin the development, run `npm start` or `yarn start`.
      To create a production bundle, use `npm run build` or `yarn build`.
    -->
  </body>
</html>
```
This is a regular HTML file as can be seen. We can edit the title to suit our needs. Simply change the `React App` text enclosed in the `<Title>` tags to whatsapp clone.

```diff
-<title>React App</title>
+<title>Whatsapp Clone</title>
```

The public folder contains assets that we do not want to change. When we will finally prepare app for production `create-react-app` will place those assets ina  build folder and reference them into HTML template.

TODO: Look at manifest.json
and follow along original manual and look at files.

