## Workshop 06 - UIElements

**What is a UIElement?**

Is an object that the user can interact with in some way.
They can e actions or outlets:
+ Action - creates a function that performs an action when tapped
+ Outlet - is a container (something else controlls the change that happens to the view)

**What does UI stand for?**

User Interface

**What symbol signals that a connections has been broken in your View Controller Class?**

A red sign will pop-up, like an error. menaing that tehre is somethinbg wrong with the calass Eg (change the camel casing conection will be broken and program will not run)
Class is not key vakue not coding complient

**How can you reconnect a broken link on a UIElement from your View Controller Class to the storyboard?**
debug are look for complient line
select view controller, go to conection onspector (circle with arrow). Orage triangle delete it.

**What symbol signals that a connections has been broken in your Storyboard Connections Inspector?**

Little orange triangle

**How to remove a broken connections in the connections inspector?**

click on object in view crontroller

**How to link a UIElement to View Controller class?**

control and drag

**How to embed a navigation controller?**

Editor, embed in, naviagtion cotroller

**Where to keep local images within your project?**

In . the assests folder

**Describe an IBAction?**

+ Action - creates a function that performs an action when tapped

**Desicbe an IBOutlet?**

+ Outlet - is a container (something else controlls the change that happens to the view)

**Label the following elements as outlets and/or actions (it might be useful to add snippets of code in here):**

+ Slider both outlet and action

The action is the motion of sliding the slider and flicking between values. 
```@IBAction func didSlide(_ sender: Any) {
  }
  ```
  
The outlet is the final value created from the action of the slider.  
```@IBOutlet weak var sliderValue: UISlider!
```

+ Button is a n action ctrolled by the user, this action is than called and the interface does the rest

Because it is 'doing' something it is an IBAction which will create a function for you. 
Your understanding of how functions 'doSomething' should help with this: 

```swift

  @IBAction func buttonTest(_ sender: Any) {
  
        //doSomething
        
  }
  
  ```

+ Label

Is a text container. 

    ```
    @IBOutlet weak var testLabel: UILabel!  
    ```

Either you can set it from the start and use it as a title or description for example. 

Or you can use a function to manipluate the text in the label (you can look at the fundamentals workshop demo for exmaples of this). 


+ Progress Bar 


+ Image View 

Allows you to place images on your view. 

The image view is simply the container for your image not the image itself. 
This allows you to flick between images using the same frame/container. 

Storage for images on device are kept in the assets folder. These images are usually used for design purposes. For example you might want an image background. 
(Accessing photolibrary and using pictures you take with camera will come later on. )

You can access the images in the assets folder by using this snippet of code and calling the name of the image you want (REMEMBER it is case and space sensitive!)

```swift
imageView.image = UIImage.init(named: "surf")
```

