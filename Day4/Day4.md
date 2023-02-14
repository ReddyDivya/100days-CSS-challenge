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
     
  


  
