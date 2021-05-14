
A Breautiful component to display display profile pictures , with animation on hover

## Demo Link <br/>
<h>https://guhankesav.github.io/react-face-component-test/<h/>

<br/>
<br/>


## Code :

### facecomponent.css

### facecomponent.jsx
```jsx
import React from 'react';
import './face.css';
import { useState } from 'react';

import face1 from './../assets/images/face1.png';

function compress(){ 
    var x = document.getElementById("ltt_lecture_dp_id")
    var cir = document.getElementById("ltt_lecture_dp_circle_id")
    var sq = document.getElementById("ltt_lecture_dp_square_id")
  
    sq.style.marginLeft= "-108px"
    sq.style.marginTop = "-219px"
    sq.style.transition=" margin 1s"
  
    
    cir.style.marginLeft="97px"
    cir.style.marginTop = "-211px"
    cir.style.transition="margin 1s"
  
  
    x.style.borderTopLeftRadius="30px"
    x.style.borderTopRightRadius="30px"
    x.style.borderBottomLeftRadius="30px"
    x.style.borderBottomRightRadius="30px"
  
  
  
  
    
  }
  function decompress(){ 
    var x = document.getElementById("ltt_lecture_dp_id")
    var cir = document.getElementById("ltt_lecture_dp_circle_id")
    var sq = document.getElementById("ltt_lecture_dp_square_id")
   



    sq.style.marginLeft="0px"
    sq.style.marginTop = "-305px"
    sq.style.transition="margin 2s"//top
  
    cir.style.marginLeft="0px"
    cir.style.marginTop = "-0px"
    cir.style.transition="margin 2s"
  
    x.style.borderTopRightRadius="70px"
    x.style.borderBottomLeftRadius="70px"
  
  
  
  
  }
const  face=()=>{



    
    return (
        <div >
              
                <img id="ltt_lecture_dp_id" className="ltt_lecture_dp" src={face1} onMouseOver={() => compress()} onMouseOut = {() => decompress()}></img>
                <div id= "ltt_lecture_dp_square_id"className="ltt_lecture_dp_square"></div>
                <div id="ltt_lecture_dp_circle_id" className="ltt_lecture_dp_circle"></div>
        </div>
    )
}
export default face;
```
## To be added in package.json
  <li>"homepage":"http://guhankesav.github.io/react-face-component-test"<br/>
    <li>"scripts": {<br/>
    "predeploy":"npm run build",<br/>
    "deploy":"gh-pages -d build",<br/>
  },<br/>
   <li>"devDependencies": {<br/>
    "gh-pages": "^3.1.0"<br/>
  }<br/>
  
## Commands :<br/>
git init<br/>
git remote add origin https: <br/>
git status<br/>
git add .<br/>
git commit -m "ini commiy"<br/>
npm run deploy<br/>
git push -u origin master<br/>

## In case of origin prob :<br/>
git remote rm origin

