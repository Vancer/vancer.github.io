<div id="cs"></div>

# CanvasSlider
> Lorem ipsum dora explora Lorem ipsum dora explora Lorem ipsum dora explora Lorem ipsum dora explora


## Methods Available

- [mySlider.init()](CanvasSlider/canvas-slider.md?id=cs-i-di)
- [mySlider.init(int min,int max, String title)](CanvasSlider/canvas-slider.md?id=cs-i-iwp)
- [mySlider.getValue()](CanvasSlider/canvas-slider.md?id=cs-rv)

<div id="cs-co"></div>

## Create object 
Lorem ipsum <code>dora explora</code> Lorem ipsum <code>dora explora</code>

```       
CanvasSlider mySlider; 

void setup(){ 

} 

void loop(){ 

}
```

<div id="cs-i"></div>

## Initialize
> Example final code

<div id="cs-i-di"></div>

* #### Default Initialization
Use <code>mySlider.init();</code> as follows:

	```
	void setup(){  
		mySlider.init();
	} 
	```


<div id="cs-i-iwp"></div>


* #### Initialization with parameters
Use <code>mySlider.init(int min,int max, String title)</code> as follows:
	```
	void setup(){  
		mySlider.init(0,100,” Temperature meter”); 
	} 
	```


<div id="cs-rv"></div>

## Reading value 
* #### Reading value from slider
Use the <code>mySlider.getValue();</code> method as follows:
	
	```	
	void loop(){ 
		mySlider.getValue(); 
	}	 
	```

<div id="cs-cec"></div>


## Example Code (Control LED Brightness)
> Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum Lorem ipsum 

	CanvasSlider mySlider; 
	int const LED_PIN = 9; 
	void setup(){ 
		mySlider.init(0,1023,” LED Brightness”); 
		pinMode(LED_PIN,OUTPUT); 
	} 
	void loop(){ 
		int sliderValue = mySlider.getValue(); 
		analogWrite(LED_PIN, sliderValue); 
	} 


