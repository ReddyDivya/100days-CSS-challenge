## 003 - The Pyramide

## Declaring global CSS variables

  - :root can be useful for declaring global CSS variables
  
  ### Syntax
      
      :root {
          --main-color: hotpink;
          --pane-padding: 5px 42px;
        }
        
      h1
      {
        background: var(--main-color);
        padding: var(--pane-padding);
      }  
---  

## CSS clip-path Property

  - The clip-path CSS property creates a clipping region that sets what part of an element should be shown.
  - Parts that are inside the region are shown, while those outside are hidden.
    
        img {
            clip-path: circle(50%);  //Clip an image to a 50% circle.
          }
      
   - circle() - Defines a circle using a radius and a position.
          
        ## Syantax
        
          clip-path : circle(length at closest-side farthest-side);
        
        ### closest-side
        
        Uses the length from the center of the shape to the closest side of the reference box. For circles, this is the closest side in any dimension.

        ### farthest-side
        
        Uses the length from the center of the shape to the farthest side of the reference box. For circles, this is the closest side in any dimension.

          clip-path: circle(90px at 90px 90px); 
          clip-path: circle(6rem at 12rem 8rem); 
          
   - polygon() - Defines a polygon using an SVG filling rule and a set of vertices.
      
---

## CSS cubic-bezier()

  - The cubic-bezier() function defines a Cubic Bezier curve.
  - A transition effect with variable speed from start to end.
  - A Cubic Bezier curve is defined by four points P0, P1, P2, and P3.
  - P0 and P3 are the start and the end of the curve and, in CSS these points are fixed as the coordinates are ratios.
  - P0 is (0, 0) and represents the initial time and the initial state, P3 is (1, 1) and represents the final time and the final state.

  ### syntax
      
      x1,y1,x2,y2	Required. Numeric values. x1 and x2 must be a number from 0 to 1
      
      transition-timing-function: cubic-bezier(0.1, 0.7, 1.0, 0.1);
   
---
## CSS Animation
    
   - CSS allows animation of HTML elements without using JavaScript or Flash!
   - An animation lets an element gradually change from one style to another.
   - You can change as many CSS properties you want, as many times as you want.
   - To use CSS animation, you must first specify some keyframes for the animation.
   - Keyframes hold what styles the element will have at certain times.

  ### The @keyframes Rule
  
   - When you specify CSS styles inside the @keyframes rule, the animation will gradually change from the current style to the new style at certain times.
   - To get an animation to work, you must bind the animation to an element.
   
   ### Example
   
     /* The animation code */
    @keyframes example {
      from {background-color: red;}
      to {background-color: yellow;}
    }

    /* The element to apply the animation to */
    div {
      width: 100px;
      height: 100px;
      background-color: red;
      animation-name: example;
      animation-duration: 4s;
    }
  
---
## SASS Variables
  
  - Variables are a way to store information that you can re-use later
  - With Sass, you can store information in variables, like:
      strings
      numbers
      colors
      booleans
      lists
      nulls
  - Sass uses the $ symbol, followed by a name, to declare variables
  
   ### Syntax
   
      $variablename: value;
      
   ### Example
   
      $myFont: Helvetica, sans-serif;
      $myColor: red;
      $myFontSize: 18px;
      $myWidth: 680px;

      body {
        font-family: $myFont;
        font-size: $myFontSize;
        color: $myColor;
      }

      #container {
        width: $myWidth;
      }
      
 ---
 
 ## SASS Variable Scope
 
  - Sass variables are only available at the level of nesting where they are defined.
  
  ### Example
  
    $myColor: red;

    h1 {
      $myColor: green;
      color: $myColor;
    }

    p {
      color: $myColor;
    }  
---

 ## Using SASS !global
 
 - The default behavior for variable scope can be overridden by using the !global switch.
 - !global indicates that a variable is global, which means that it is accessible on all levels.
 
 ### Example
 
     $myColor: red;

      h1 {
        $myColor: green !global;
        color: $myColor;
      }

      p {
        color: $myColor;
      }
 
