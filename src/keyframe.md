# Keyframe

![Keyframe](./image/keyframe.jpeg)

*A transition is conceptually similar to a keyframe animation: You define the first frame (starting point) and the last (ending point), and the browser computes all the intermediate values so the element can transition smoothly between them. With keyframe animation, however, you’re not limited to defining only two points. You can define as many as you like. The browser fills in the values from one to the next to the next, until it reaches the final keyframe, producing a series of seamless transitions.*

<style>
    @keyframes over-and-back {         
        0% {
            background-color: hsl(0, 50%, 50%);
            transform: translate(0);           
        }

        50% {                                
            transform: translate(200px);
        }

        100% {                                   
            background-color: hsl(270, 50%, 90%);  
            transform: translate(0);               
        }                                        
    }

    .box {
        width: 100px;                             
        height: 100px;                            
        background-color: green;
        animation: over-and-back 1.5s linear infinite;
    }
</style>

<div style="height: 250px">
    <div class="box"></div>
</div>