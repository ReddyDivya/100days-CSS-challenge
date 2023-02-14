## Day 4 

## CSS Box Shadow

  - The box-shadow property attaches one or more shadows to an element.
  
    ### Specify a horizontal and a vertical shadow

       ### Example

        div {
            box-shadow: 10px 10px; /* Horizontal Vertical */
          }
          
     ### Specify a Color for the Shadow
       
       - The color parameter defines the color of the shadow.
       
       ### Example
        
        div {
          box-shadow: 10px 10px lightblue; /* Horizontal Vertical Color */
        }
        
     ### Add a Blur Effect to the Shadow
     
      - The blur parameter defines the blur radius. The higher the number, the more blurred the shadow will be.

      ### Example 
      
        div {
          box-shadow: 10px 10px 5px lightblue; /* Horizontal Vertical Blur Color */
        }
        
     ### Set the Spread Radius of the Shadow
     
      - The spread parameter defines the spread radius. 
      - A positive value increases the size of the shadow, a negative value decreases the size of the shadow.
      
        ### Example
        
            div {
              box-shadow: 10px 10px 5px 12px lightblue;   /* Horizontal Vertical Blur Spread-radius Color */
            }
            
     ### Set the inset Parameter
      
       - The inset parameter changes the shadow from an outer shadow (outset) to an inner shadow.
        
       ### Example
       
        div {
          box-shadow: 10px 10px 5px lightblue inset; /* Horizontal Vertical Blur Spread-radius Color inset */
        }
---        

## CSS animation - shorthand
  
  - The animation shorthand CSS property applies an animation between styles. 
  - It is a shorthand for animation-name, animation-duration, animation-timing-function, animation-delay, animation-iteration-count, animation-direction, animation-  fill-mode, and animation-play-state.

    ### Example
    
        /* animation-name animation-duration animation-timing-function animation-delay animation-iteration-count animation-direction*/
        
        $bezier: cubic-bezier(.21,.98,.6,.99);
        
        animation: jump-jump-1 2s $bezier infinite alternate; /* name duration timing-function delay iteration-count direction*/
  
---
## CSS animation - animation-fill-mode

  - The animation-fill-mode CSS property sets how a CSS animation applies styles to its target before and after its execution.
  
  ## Syntax
  
    animation-fill-mode: none;
    animation-fill-mode: forwards;
    animation-fill-mode: backwards;
    animation-fill-mode: both;
    
   ### forwards 
     
   - The target will retain the computed values set by the last keyframe encountered during execution. 
   - The animation will be applied and won't come to it's origin.
   
   ### backwards 
   
   - The animation will be applied and comes back to it's origin.
   - The animation will apply the values defined in the first relevant keyframe as soon as it is applied to the target, and retain this during the animation-delay period.

   ### both
   
   - The animation will follow the rules for both forwards and backwards, thus extending the animation properties in both directions.

   [Demo](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-fill-mode)

---

## CSS animation - animation-delay

  - The animation-delay CSS property specifies the amount of time to wait from applying the animation to an element before beginning to perform the animation. 
  - The animation can start later, immediately from its beginning, or immediately and partway through the animation.
  
  ### Example
  
     animation-delay: 3s;
    
  [Demo](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-delay)

---  

## transform: scale()

  - The scale() CSS function defines a transformation that resizes an element on the 2D plane.
  - It can resize the horizontal and vertical dimensions at different scales.

  ### Example
  
    transform:scale(1);
    transform:scale(0.7);
    transform: scale(1.3, 0.4); /* Horizontal Vertical */
    transform: scale(-0.5, 1); /* Horizontal Vertical */
    
  [Demo](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/scale)

---  
  


  
