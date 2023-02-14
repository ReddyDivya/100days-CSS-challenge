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


  
