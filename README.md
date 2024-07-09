0.- npm install -g capacitor
0.5.- npm install @capacitor/core @capacitor/cli@latest @capacitor-community/electron
1.- npm install ngx-electron electron   (tambien    npm install electron --save-dev)
2.- npm install electron-packager (empaquetar para ejecutar en SO)
2.3.- npm cache clean --force
2.5.- npm install
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

En git bash escribir: curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
Encontrar donde se instaló

Ve al menú Archivo -> Preferencias -> Configuración.

En la barra de búsqueda de configuración, escribe terminal.integrated.env.windows.

Añade la ruta completa de la carpeta bin de nvm al valor de PATH. Por ejemplo: C:\Users\Franc\.nvm
)
