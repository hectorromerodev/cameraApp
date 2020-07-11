# Example - USING CAPACITOR CAMERA

### How to start

Create a project and add capacitor to our project
  1. ionic start cameraApp blank --type=angular
  2. cd cameraApp
  3. npm install --save @capacitor/core @capacitor/cli
Add application name, appID and platforms to use
  1. npx cap init
  2. ionic build
  3. npx cap add android (to add android) 
We need to add pwa-elements to avoid ( TypeError: cameraModal.present is not a function )
  1. npm install @ionic/pwa-elements
  2. add this on main
      import { defineCustomElements } from '@ionic/pwa-elements/loader';
      defineCustomElements(window);
Add UI Elements
