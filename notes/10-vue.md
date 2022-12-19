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



always route the new page that you have created

<!-- if using the ref in setup, you must access the value -->

<!-- reactive is meant for objective -->


const router = useRouter()


note emit is black magic and should only be used in very rare cases aka not friday
because data goes downwards not upwards








always have inside setup the prop..
EX: setup(props) {



condtionals

being able to delete if your the creator


drawing data to the page

being able to post

account info(username and logo)

on the component


using sandbox


change env.js
 to codeworks


 run npm i


making sure account comes back @200


get the data in services in console log


using an api that you didnt write make a model



get raw data to draw on page

 v-for, for each "thing" in collection

when making the card
use props
  props:{
type: model name
required
 }
 in homePage
<prop name : prop name = "random lettter">


 to use computed in css

.class name{
  the styles you want
  by calling it in a 
  backgroundImg: v-bind(coverImg)
  v-bind binds  a property injects

}

setup(props)
in return write a compute
coverImg; computed(()=> 'url'(${${props.model.theimg}))




make a profilePage

then make a rout
path: '/profile/profileId',
name: '/profile',
component: loadPage('profilePage')
<!-- make sure to store id in path -->


in projectCard

router-link :to="{name: 'profile', params: {profileId: projects.creator.id} }"

in profilePage
setup(){
  const route = useRoute()
  <!-- make a profile service -->
  in service 
  async function getProfileById(route.parms.profileId){
try{
}

  }
}
make an onMoubted(() =>{

})


after getting the data
store in appState

activeProfile = null


add additinoal propeirtes in account model for the active profile


in account service

appstate.account = new Account(res.data)

v-if="profile", render on page if theres one



async function getProjectsByCreatorId(){
await projectService.getProjectsByCreatorId(route.params.profileId)
}

in services 

async function getProjectsByCreatorId(creatorid){
const res = await api.get('api/projects', {params: {creatorId: creatorId} })
<!-- line above makes it like a query -->
}


in login component


make a new router-LINK - 
for profile page





<!-- before enter: authGuard
check if their logged in
if not
prompots log in page -->



const editable = ref({})
watchEffect(()=> {
  if(appState.account,id){
    editable.value= { ...appState.account}
  }
})










one to mmany

albums and creator


one to many

pictures in an album

many to many

collaberators



post man tests



bcw crate fullstack vue!!!


client on 8080
server on 3000


first step fill out the .env


make a model first 


export const BlankSchema = new Schema({

})

enum: it has to be one of these values

dont change post man things
only the add token



for one id 


locall/api/blank/{{blankId}}



post, get, findbyid, archrive or delete 




npm in server and client folder


cd in client 


to filter 


in the computed 

if{filterBy.value ==''}
return appsate.blank



else{
  return Appstate.blank.filter(a => a.catogaery == filterBy.value )
}


account is personal


profile is everyone else.



link component in homepage

or inject it somewhere


modal content
<slot><slot>



blank component 
inject component in here
blank component



router moves people through pages


in auth0 services, add in the function you want to happen before user is logged in

