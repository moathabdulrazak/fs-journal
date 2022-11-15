# MVC


<!-- blank keyword is function -->

mvc group code that does certain things togather

view is html, dom
what the user sees
html represenation of the data in the app


c is controller
takes in action from user
draws data to dom
the only thing user has access to

service bussiness logic happens
bussins logic is anything that modifes data


appstate is the single source of truth or where all the apps data will be stored



model blue print of what the data in the appstate will look like



app.js

as long as you export it, you can import.


start with model to build data

start with constructor  (name, blank, blank, blank){
  <!-- constuctor in model, is the data  -->

  this.name = name
  this.blank = blank
  this.blank = blank
  this.blank = blank
}
get nameTemplate(){
  reutrn `html data ${this.name}`
}

blank

app.js is the door to the index code
under class app{
  namesController = new NamesController() import data
  this.drawNames
}

then in appstate store the model

blank = [
  new blank (data goes in here such as name, price or score.)
  new name( data goes in here )
  has to be a string inside the data ''
]

<!-- services and controller are handling all the "data" -->
then go into controller


export class namesController

in controller
drawNames(){
  let noms = appState.names
  let template = ''
  noms.foreach(m => template += m.name)
in controller im port setHtml('name-list', template)  
}




services 

class namesServices{

}

export const nameService = new NamesService(){
  contrucotr (){

  }
}



in utlity writer,
export function setHTML(id, html){
  getElm(id).innerHtml = html
}


selectable class, makes a easy looking hover


in model



appstate.on('data', this draw function) register a listiner
not passing a function so no(), inovked right away.








<!-- controller listens to insturction from the appstate -->

... takes away space from an array

[...appState.myMoney, mon]



<!-- make a controller and service -->

<!-- create a controller or service, add in app.js -->




create a model, step 1. set up your model.consttrcutor is building the class or model.
(model data in construcor)
after model import it to the appstate


step 3, build out a template for our model


step 4, place template on model.

get cardTemplate(){
  return `template in here`
}

step 5, create a controller with a console log in the constructor
step 6, register controller in the app.js and get your console log om your web page.

in controller
first step in controller always log

in constrcuor function runs on page load in controller

in app blankController = new blanksController()

anything outside the controller user cannot access

_drawBlank(){
  let template = ``
  appState.blank.forEach(c => template += blankTemplate)
  setHtml ("id", template or value)
  }

  in constructor call it, _drawBlank()

  <!-- appState.on will call a method, everytime in the appstate something changes. -->

  <!-- just drawing it regularly would draw it automaticlly on page -->

  step 7 update our template with fields from the class



  <!-- this refers to the instance of the class -->


delete button
  onclick="app.blankController.removeBlank('this.id')" title="remove blank" in html

  in controller 

  <!-- removeBlank(){
 pop.toast("message", "info") (make sure to import)
  } -->
 async removeBlanl(){
    if(pop.comfrim)('are you sure want to remove blank){
      blanksService.removeBlank() hit control peroid then it will declare remove car
    }
  }
<!-- async click on button for code to move on
only use await/async for pop.confrim this week  -->

<!-- sweetalert.com  cool utility to use-->
  utility pop, makes it easier to use sweetalert utilty

step 8 when you need to change data in the appstae, write out your service

  in service

  removeBlank(blankId){
    <!-- give me a new array of blanks where all of blanks id's do not match  the id i passed down-->
    let filteredArray = appState.blank.filiter(c => c.id ! =carId)
   appState.blank = filitredArray
  }



  in model in the construcotr
  create an id 
  this.id = generateid()
  <!-- in utility, import the generate id -->
  <!-- generateid generates random string, on page loads. asign uniqe ids to each data point -->


  pass id in remove button


appstate.on('cars', _drawCars)

ita better to draw in constrctuor as appstate, for less code


<!-- forms -->
required in input field
in html
form onsubmit"app.blankController.createBlank"
first step to build a form
div
inside div
create a form
go to bootstrap grab a form
paste
change type 
label for would be make
placeholder would be make
inside label make
change form elements to match (this.blank)
change price type to number
button submit
in html add name ="make"
add in all input feields after the placeholder
<!-- name property match something in model -->
button type reset, resets the form
button type submit, submits
for image change type to url

floating textareas for description


<!-- m-auto moves to center of page -->

in controller


createBlank(){
  <!-- allows it to not fresh page -->
  window.event.preventDefault()
  <!-- targets the form -->
  let form = window.event.target
  <!-- grabs form data -->
let formData = getFormData(form)
blankService.createBlank(formData)
}

<!-- form handler utlity.  -->


in service

createBlank(FormData){
  let newBlank = new Blank (formData) (make sure to import)
  appState.blanks = [..appState.blanks, newBlank]
}



details modals



modal is hidden until needed, put underneaht the footer.







need data-bs-toggle and data-bs-target

go into model paste in button class


add onclick in button 
onclick= "app.blanksController.setActiveBlank('${this.id})"


active

in controller

setActiveBlank(blankId){
  blanksService.setActiveBlank(blankId)
}



in service
setActiveBlank(blankId){
  let foundBlank = appState.blanks.find(b => c.id == blankId)
  appState.ActiveBlank = foundBlank
}


to setActive
in appState
import singular model/blank
activeBlank = null

controller
write a function -drawActiveBlank
in constructor draw _drawActiveBlank



in model we set a new template

in modal hard code in html to use in template


getActiveBlank(){
  return`template`
}

throw id in modal content


controller 
function _drawActiveBlank(){
  setHTML("id", appState.ActiveBlank.ActiveBlankTemplate)
}



go into model
this.createdAt = new Date()
in string inerpaltion
this.createdAt.toLocalDalestring




local storage

in  service
createBlank function
and removeBlank
saveState('blank', appstate.blank)


in appstate

blank = loadState("blank", [blank(array)])

<!-- store utility save state and load state -->

in our save state we need to give it a (key (id)   )




in constructor keep the DrawHouse function
till you dont want it to draw right as page starts



in model

static GetBlankFormTemplate(){
return ``
}



model
constructor (data)
this.blank = data.blank
this.date = data.date || new Date()
<!-- creates date that happens when it was  submitted -->

after model create instance in appstate

<!-- build out modal, and test data. -->


get computeBlank(){
  return this.blank.slice(0, 15) + '...'
}


forms alwyas need to have a input, id and name

map()
<!-- map creates a copy of the array with actions performed on it. -->




<!-- make an active template -->








<!-- asynchronous code -->


wait allows it for useer to makke a descison in the aycync


await and aysnc pause code till we get result from user


promise makes sure that something comes back

api = application progamming interface


taking request and dumb out data


in console, network shows you what the api data has

api gets you JSON 

dont start with model

if we didnt create the data, dont start with the model



app.js drop the controller

start with controller
async getBlank(){
await blanksService.getblank()
}


<!-- fetch, grabs in a url -->
drop api url as a string
<!-- http.cat -->


const data = await reponse.json()
fetch method


appstate
cards = []
since the data doesnt exist since we didnt create the data
so its an empty array


in html
script axios

in service 
const response = await axios.get('api url in here')

<!-- axios is not here when writing the code, but here after its loaded by html
dont load in service. its loaded in htmls -->



in controller

function draw cards()
let cards = appstate.cards
let template = ''
cards.foreach(c => template += c.name)
sethtml('app', tem[late])

appState.on('cards', draw cards)


to convert data 
use map (cardData => new card cardData)


try catch

try doing this thing
if not catch error 

