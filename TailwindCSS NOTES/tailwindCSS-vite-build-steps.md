# Steps to get the Production Build of TailwindCSS Using Vite build.

- In `package.json` file, Change scripts to this..
```
"scripts": {
    "start": "vite",
    "build": "vite build"
  },
```

- In the Terminal, write the below code and press `Enter`

```
npm run build
```

- A `dist` folder will be generated. This is the final output of the production with the smallest size of the files.
- Drop & Use this folder at websites like netlify to deploy your Dynamic tailwindCSS Website.
