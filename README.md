# Tezjs with Google-Fonts

- Create fresh Tezjs project 

- Now add one **add-lib.ts** file under root directory.

- For add particular google-fonts in your project add your import **addLib** and **addStylesheet** modules from @tezjs/js in your add-lib.ts file

```
  import { addLib,addStylesheet } from "@tezjs/js"
```

- After that export one function with option **afterUserInteraction** and add your stylesheet under **addStylesheet** function same as below.

```
export default addLib({
    afterUserInteraction:[addStylesheet("https://fonts.googleapis.com/css2?family=Dancing+Script:wght@500&family=Passion+One&display=swap")]
})
```

- Now add your font family inside **assets/index.css** with html json same as below 

```
  html{
    font-family: 'Dancing Script', cursive;
    font-family: 'Passion One', cursive;
}
```

- Now check your fonts on output it's replaced with new font family