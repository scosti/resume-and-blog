---
author:
  name: "Stefano Costi"
date: 2023-01-20
linktitle: Why contribute to an open source project ?
type:
- post
- posts
title: Why contribute to an open source project ?
weight: 10
series:
- Hugo 101
---

## Intro
Hugo is a light and fast framework for buil static website like this one! 
If you want a platform for build and autmatically deploy a hugo website in cloud, Netlify it maight be the best choice for you. 
I was suddenly affascinated when I saw that Netlify gives you the ability of speed up and take control of your delivery process. 
Moreover in this platform you have configurable piplines and many serverless services as well.

### My first pull request in a open source project
My first pull request was about animate the logo in the menu bar of this Hugo theme. 
if you click in different pages, the path displayed will changed. After some days the PR was accepted and it was meged in master.

Here some of the javascript,
this code concatenate the page url with the logo text `logo.textContent`. The event `window.onload` is fired when new window is loading.
```
const language = document.getElementsByTagName('html')[0].lang;
const logo = document.querySelector(".logo__pathname");
if(logo){
  window.onload = () => {
    let path = window.location.pathname.substring(1);
    path = path.replace(language+'/','')
    logo.textContent += path.substring(0,path.indexOf('/'));
  };
}
```
### Why contribute to an open source project ?
When I approached to the project of this website I was wondering if is better a ready-to-use theme or make it by myself.
Actually i found out the best solution was use a Hugo theme and contribute to the open source project.
Surely this is an opportunity that gives a lot of value to your project.
I was exited to contribute to a Github project, definitly it was the best choice. I learned the importance of sharing new functionalities because many people will use them in future. Now I know that open surce is the right approach for grow a product strongher. I hope to continue to add value to the open source community. 
