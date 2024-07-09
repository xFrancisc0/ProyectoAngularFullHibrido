0.- npm install -g capacitor
npm install -g @angular/cli 
npm install -g @ionic/cli
0.5.- npm install capacitor @capacitor/core @capacitor/cli@latest @capacitor-community/electron
1.- npm install ngx-electron electron   (tambien    npm install electron --save-dev)
2.- npm install electron-packager (empaquetar para ejecutar en SO)
2.3.- ionic start IonicElectronApp blank --type=angular

Dentro de proyecto:
3.- ng serve (Probar aplicaciones)
4.- ctrl+c
5.- ng build

Crear capacitor.config.json
{
    "appId": "com.example.app",
    "appName": "ProyectoAngularFullHibrido",
    "bundledWebRuntime": false,
    "webDir": "./ProyectoAngularFullHibrido/proyecto-angular-full-hibrido"
}

Fuera de proyecto:
npx cap init ProyectoAngularFullHibrido com.example.myapp
npx cap add electron
npx cap open electron

(En caso de error
Eliminar la carpeta electron
npm update @capacitor/core @capacitor/cli @capacitor-community/electron
Remove-Item -Path .\electron -Recurse -Force
Borrar capacitor.config.ts dentro del proyecto
npx cap init ProyectoAngularFullHibrido com.example.myapp
npx cap add electron
npx cap open electron

En git bash escribir: https://4geeks.com/es/how-to/como-instalar-nvm-en-windows (coreybutler/nvm-windows)
Instalar ultima version de node: nvm install 20.15.1
Instalar el node que nos sirve para ionic-electron app: nvm install 18.20.4
Instalar npm: https://docs.npmjs.com/downloading-and-installing-node-js-and-npm


Usar node que nos sirve: nvm use 18.20.4
)
