## PROJECT GoodNewa.

WHAT IS GOING TO BE BUILT:
News app that receives the new from the [News API](https://newsapi.org/docs/endpoints/top-headlines) .

### MVVM on the project:

At the Web service implementation, the service receives  data from the API, so to follow MVVM it can not interact with the View Model directly. Thats why the model is implemented.

## ARCHITECTURE PATTERNS

### MVC Architecture

* Model:
Data in the application. 

* View:
User Inteface. What the user sees on the screen. With what the user interacts.

* Controller:
Communicates the model with the view. Intermediate between Model and view.

* Contras (Practices that lead to ***bad code***)
Overfloding the controller with code. Making sure that they Model and View are separate. Having to much code difficults testing process.

### MVVM Pattern:

* View:
User Inteface. What the user sees on the screen. With what the user interacts.

* ViewModel:
Data that is going to be binded (attached) to the view.
Supplies the data to the view.

View talks to the *ViewModel* but does not talk to *Model*

* Model:
Bussiness logic. 

*ViewModel* and *Model* communicates between each other.

Lean Controllers:
Purpose have less code on the cotrollers.


## VIEW IMPLEMENTATION KNOWLEDGE
### NAV BAR UI:

* Editing the navBar from App Delegate so it applies to every view.

#### Colour

Change navigation bar background colour:

`UINavigationBar.appearance().barTintColor = UIColor(displayP3Red: 47/255, green: 54/255, blue: 64/255, alpha:  1.0)`
   
 Change text colour:
 
`UINavigationBar.appearance().largeTitleTextAttributes = [NSAttributedString.Key.foregroundColor: UIColor.white]`
* Large Tittle I think is mainly for static navigation bar that iphones with larger screen that my iphone 8 has to be confirmed
        
`UINavigationBar.appearance().titleTextAttributes = [NSAttributedString.Key.foregroundColor: UIColor.white]`
* Title for the scrolled screen or the normal for screen such as iphone 8.

## VIEWMODEL IMPLEMENTATION KNOWLEDGE

## MODEL IMPLEMENTATION KNOWLEDGE

### Struct

* Structures in swift are maily used to model tibutes of an object

#### Decodable
Used to modeled object that want to be only decoded.

#### Codable
Used to modeled objects that are going to be decoded and coded. Mainly when you want to retrive the object to the server.

