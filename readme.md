# jswindow
### How to use:
Define the window, you can specify the title and icon url here (optional):
```
var eg = new jswindow({title: "", icon: ""});
```
Open the window, you can specify the width, height, and distance from left and top, in px (also optional):
```
eg.open({width: 100, height: 100, left: 100, top: 100});
```
Close the window:
```
eg.close();
```
Access the window:
```
eg.innerWindow.innerHTML = "something";
```
More things you can use:
```
eg.onclose
eg.setTitle("String")
eg.setIcon("String")
```

### Example
```
var eg = new jswindow({title: "Window", icon: "https://assets.stickpng.com/images/580b585b2edbce24c47b2a2c.png"});
eg.innerWindow.innerHTML = "<h3>Hi there!</h3>";
eg.onclose = function() { console.log("The window was closed!"); }
eg.open({width: 400, height: 100});
```