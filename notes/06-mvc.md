# MVC

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