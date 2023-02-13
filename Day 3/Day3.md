## 003 - The Pyramide

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

  A transition effect with variable speed from start to end
   
