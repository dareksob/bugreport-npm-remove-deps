# BugreportNpmRemoveDeps

This is a simple angular setup that dependece on thirth part package located on github.
Example that can reproduce the bug if you add new package by npm.

## Bug
Remove dependency packages if you add new package.

## Steps
1. init project by install it. npm i
2. run it, every looks fine
3. add new package by npm 
```
npm i angular-oauth2-oidc
```
Now you can a message

````
 angular-oauth2-oidc@4.0.2
added 2 packages and removed 101 packages in 14.394s
````
They remove the dependecy @deepblue/stylekit and the application cannot work anymore.