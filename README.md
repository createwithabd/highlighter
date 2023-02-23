# Highlighter  

Build by `Abdullah Amjad` 

A small module that allows you to customize print statements or output text with different colors. You can use any color type from the following `xterm`, `rgb`, and `hexa` to select a color for your output text. 

## Requirements: 
1. Python version >= `3.8.10`

## Dependencies
This project has no dependencies till now and can be used with `windows`, and `Linux` operating system. 

## Installation
You can install it by running following command on your terminal.
~~~bash
pip install highlighter
~~~
OR 
~~~bash
pip3 install highlighter
~~~

## Usage

To use this package, import `log` method from `highlighter` inside your required python script .

~~~python
from highlighter import log
~~~

Now, you can use `log` to output colored text on terminal. 

**For Example:**

~~~python
from highlighter import log
log.message("My first message using this package.")
~~~

### Output

![log.message](./images/log_message.png)





## Features 

I build this module with flexibility to select any color type between `xterm` bit integer, `rgb` color tuple and `hexa` color code. You can use any color type to customize the output text on your terminal. There are some default methods as well which you can directly use to output respective text. Those methods are as follow; 

1. `log.message()` - You can put any string inside the curly brackets to display your text on the terminal. Default color is `put color`. 
2. `log.error()` - You can use this method to output `ERROR` on your terminal. 
3. `log.warning()` - You can use this method to output `WARNING` on your terminal. 
4. `log.success()` - You can use this method to output `SUCCESS` status on your terminal. 
5. `log.info()` - You can use this method to output any kind of important `INFO` on your terminal. 
6. `log.highligh()` - If you want to highlight any specific part in your print statement then, you can use this method inside the `f-string` or `.format` option of print statement.  



#### Options: 
1. `text` - Can provide any string value. **Default:** `None`. 
2. `color_type` - Can provide any color type from `xterm` , `rgb` and `hexa` . **Default:** `xterm`
3. `fg` - Can provide any foreground color with respect to its color type. For Example: 
   - For `xterm` - you can provide any integer between `1 and 255`
   - For `rgb` - You can provide `rgb` tuple `(r, g, b)`. 
   - For `hexa` - You can provide HEX color code `#000000`

4. `bg` - Same as foreground color you can provide any value with respective to `color_type` argument. 
5. `prefix` - Can be used in special method like `log.error()` - Prefix = `True` will display `[ ERROR ]` prefix at start of your output text. **Default:** `False`. 
6. `tag` - Can customize prefix tag as well. **Default:** `None`. 
7. `dc` - Default color to pass an argument to a method or it can be used to set the color for your prefix tag. 



------
## Other features 

1. `rgb_to_hex(rgb:tuple=(0, 0, 0))` 
2. `hex_to_rgb(hex:str = "#000000")` 
3. `rgb_to_xterm(rgb:tuple=(0, 0, 0), val = False)`
4. `hexa_to_xterm(hex:str = "#000000" val_ = False)`
5. `custom_color_from_rgb(fg=None, bg=None)`
6. `custom_color_from_hex(fg=None, bg=None)`
7. `custom_color_from_xterm(fg=None, bg=None)`



## Contributors
----
<div class='set' > 
    <a href="https://github.com/createwithabd/highlighter/graphs/contributors">
    <img src="https://contrib.rocks/image?repo=createwithabd/highlighter" />
    </a>
</div>

------



