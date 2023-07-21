# Matrix Rain aka cmatrix

It is a simple graphical animation created using Pygame. It generates a rain-like effect on the screen by dropping random ASCII symbols from the top of the screen to the bottom. The animation is infinite, and the symbols fall at random intervals and speeds to create a visually appealing effect.

## Code Explanation
Let's briefly explain the key components of the code:

Symbol Class: This class represents an individual raindrop symbol. It randomly chooses an ASCII symbol from the green_symbols list, sets a falling speed, and updates its position on the screen during each frame.

SymbolColumn Class: This class represents a column of falling symbols. Each column consists of multiple symbols arranged one above the other. The number of symbols in each column and their falling speed are randomly determined during initialization.

Initialization: The script initializes the Pygame library and sets up the screen dimensions. It also loads the font and creates a list of green-colored ASCII symbols.

Main Loop: The main loop of the animation keeps running until the program is terminated. Within the loop, the screen is filled with a black color, and each symbol column is drawn on the screen. The loop checks for quit events to allow the user to close the window gracefully.

## Customization

You can customize various aspects of the animation to suit your preferences:

Screen Size: You can modify the WIDTH and HEIGHT variables to change the size of the animation window.

Font Size: The FONT_SIZE variable determines the size of the falling symbols.

Symbol Color: To change the color of the symbols, modify the pg.Color('green') argument when rendering the font.

Symbol Set: You can replace the symbols list with your own set of ASCII characters to use different symbols in the animation.

Speed and Frequency: The speed and frequency of falling symbols are randomly determined during initialization. You can modify the range of speed and frequency by changing the parameters in the SymbolColumn class.

# Outputs

![cmatrix - 1 - random Katakana characters cycling through](cmatrix1.gif)
![cmatrix - 2 - random Katakana characters cycling through in a single column](cmatrix2.gif)
![cmatrix - 3 - random Katakana characters cycling through in a single column](cmatrix3.gif)
![cmatrix - 4 - random Katakana characters cycling through in multiple columns](cmatrix4.gif)
![cmatrix - characters (letters and numbers) falling in a rain-like pattern](cmatrix.gif)

## References

- https://www.youtube.com/watch?v=rzA8cZyisf8 - Matrix Digital Rain in Python with Pygame -- Coder Space