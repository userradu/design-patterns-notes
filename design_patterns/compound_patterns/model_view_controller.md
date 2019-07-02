# Model-View-Controller

**Model**
- holds all the data, state and application logic. 
- the model is oblivious to the view and controller 
- it provides an interface to manipulate and retrieve its state
- it can send notifications of state changes to observers

**View**
- gives you a presentation of the model 
- usually gets the state and data it needs to display directly from the model 

**Controller**
- takes user input and figures out what it means to the model
- it lives in the middle, between the view and the model

1. The user interacts with the view. When you did something to the view, the view tells the controller what you did. It's the controller's job to handle that. 

2. The controller asks the model to change its state. The controller takes your actions and interprets them. If you click on a button, it's the controller's job to figure out what that means and how the model should be manipulated based on that action.

3. The controller may also ask the view to change. When the controller receives an action from the view, it may need to tell the view to change as a result. For example, the controller could enable or disable certain buttons or menu items in the interface. 

4. The model notifies the view when its state has changed. 

5. The view asks the model for state. The view gets the state it displays directly from the model. The view might also ask the model for state as a result of the controller requesting some change in the view.

Notes
In some designs the controller registers with the model and is notified of changes. This can be the case when something in the model directly affects the user interface controls. For example, certain states in the model may dictate that some interfaces items be enabled or disabled. In this case, is the controller's job to ask the view to update its display accordingly. 

Why not have the code from the controller in the view directly? 
You'll complicate your view code because it now has two responsibilities: manage the user interface and dealing with logic of how to control the model.
Second, you're tightly coupling your view to the model. If you want to reuse the view with another model, forget it. 
The controller separates the logic of control from the view and decouples the view from the model.  

**The patterns in MVC**

**Observer**
- the model uses Observer to keep the views and controllers updated on the latest state changes. 

**Strategy**
- the view and the controller implements this pattern. The controller is the behavior of the view, and it can be easely exchaned with at different controller if you want a different behavior
- the view is an object that is configured with a strategy. The controller provides the strategy. 

**Composite**
- the view uses this pattern to manage the windows, buttons and other components of the display
