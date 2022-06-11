# Introduction

The goal of this project is to provide a professional and easily customizable Portfolio.

No need to know anything about web development, I explain everything to you ! :blush:

# How to install

First of all, download the project or clone it:
```
git clone https://github.com/MRK4/portfolio-builder.git
```

Une fois que c'est fait, afin de pouvoir voir à quoi ressemble le site, ouvre un terminal dans le dossier racine du projet (/portfolio-builder) et faites:
```
npm run serve
```

Once this is done, open a new page in your browser and enter in the URL: `localhost:8080`.

Now you can see the website ! :tada:

# How to customize

I tagged all the possible customizable areas with the word "CUSTOMIZATION".

I will explain you step by step how to modify the components, but you can look for yourself by searching the word "CUSTOMISATION" in your IDE.

## Change your Name / Job / Details

Go to `src/components/Portfolio_Header.vue`.

From line `63` to `68`, you will be able the change the informations.

## Change your picture

Go to `src/assets/imgs`.

### Keep the .jpg extension

Simply replace the `avatar.jpg` by antoher JPG image of your choice.

### Choose another extension

Go to `src/assets/imgs` and put your image here.

Then go to `src/components/Portfolio_Header.vue`.

At line `9`, you will have:
```
<img class="outline-2 [...]" src="@/assets/imgs/avatar.jpg" alt="Profile Picture">
```

Change the `src="@/assets/imgs/avatar.jpg"` by the name of your picture.

_For example, if my picture is called `sunflower.png` I'll have to write `src="@/assets/imgs/sunflower.png"`_

## Add your work

Go to `src/components/Portfolio_Grid_Showcase.vue`.

A sample code is present from line `21` to `48`.

In order to add your work, you just have to copy the following lines and paste them after those already present.

```
{
  title: "Write the name of your project",
  img: "yourimage.jpg",
  url: "Enter the URL of your project, if there are none, leave the quotation marks blank",
},
```

**The images of your projects must be square.** _For exemple: 1000 x 1000, 2500 x 2500, 5000 x 5000, ..._

**The extension of your images is free. Please consider that for this project I have chosen to provide images in .jpg but the .webp extension will be more suitable for the web.**

## Change / Add / Remove social networks

```
WORKING ON IT PLEASE BE PATIENT...
```

## Change the colors

```
WORKING ON IT PLEASE BE PATIENT...
```

# License

[MIT License](https://choosealicense.com/licenses/mit/)

Copyright (c) 2022 MRK

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.