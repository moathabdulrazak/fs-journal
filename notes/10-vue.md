# vue



bcw create vueStarter


<!-- no more html -->


in pages where we write in vue

no controllers

but components


<!-- in homepage -->

vue template is the html
something like the get template



vue script is the javascript


style is the css

breaking up chunk of html that have html, css and javascript


<!--  -->


<!-- if it doesnt work, run npm i -->



<!-- first rule of vue, for the template to access data in the script must be in the return -->
<!-- second rule for reactivity to take place you must use vues reactive stuff -->



v-on:click
or @click

a variable in homepage should exist only if needed one



in appState if you want the function to be everywhere






v-for="number in something"
will render same sort of model


: is for interpolation in tags

{{}} is for interpolation in between tags 'contents'






onmounted(()=>)

onMounted is the vue lifecycle hook that fires when a component is loaded to the dom
simllar to constructor()




mpa = mulitpage application
spa = single page application 



first make a model

second make an axios service for the api
<!-- export const blankAPI = axios.create({
  baseURL:
  timeout:
  params:{
    api_key:
  }
}) -->

third make a service


instead of loading in controller
you can load it in a page

in setup
<!-- when awating functions try to keep the async part out of an on mounted -->
 <!-- onMounted(()=>{
getBlank
 })
 async function getBlank(){
  try 
await blanksServivce.getBLAnk
  catch
 } -->


 then  in appState make a place to store your data

 then in homepage 

 compute the appstate
  





  paginaation 

  make a secetion

div btn previous
div btn next

in homepage
in return
async changePage(){
  awaait  blanksService.changePage(2)

}

in appstate
page: 1


props are like a method that your passing an arugement throguh it


props allow you to pass elements throguh diffrentt pages

:blank=''

v-model="" what your tying into it










