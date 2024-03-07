# 01-oct-flex-in-css
Assignment of Flex-properties.
Question.1  Decribe the main differences between the css flexbox layout model and the css grid layout model. When would you choose to use one over the other?
Answer:-

It seems like you're asking about the differences between the CSS Flexbox layout and the CSS Grid layout, and when you might choose one over the other. Here's a brief comparison:

Flexbox:

Flexbox is a one-dimensional layout method for laying out items in a single direction—either in a row or a column.
It's best suited for arranging items within a container in a linear direction, allowing for easy alignment and distribution of space among items.
Ideal for components like navigation menus, lists, or elements within a container that need to be organized in a single direction.
CSS Grid:

CSS Grid is a two-dimensional layout method that allows you to arrange items in rows and columns.
It provides precise control over both the rows and columns, allowing for more complex layouts.
Grid is suitable for creating overall page layouts, especially when you need to align items in both horizontal and vertical directions.
It's also useful for creating responsive designs, as you can define different layouts for different screen sizes.
When to use each:

Flexbox: Use when dealing with layouts in one dimension, such as navigation bars, lists, or distributing items within a container.
Grid: Use when you need to create complex layouts with rows and columns, such as overall page layouts, grids of images or content, or any design that requires precise control over both horizontal and vertical alignment.

<br>
Question.2 Explain the role of the following key properties in the flexbox layout model.
1.Justify-content
2.align-items
3.Gap
4.flex-direction
5.flex-wrap
Answer:-
<big>justify-content: </big>

This property aligns flex items along the main axis of the flex container.
Values include:
flex-start: Items are packed toward the start of the main axis.
flex-end: Items are packed toward the end of the main axis.
center: Items are centered along the main axis.
space-between: Items are evenly distributed along the main axis, with the first item at the start and the last item at the end.
space-around: Items are evenly distributed along the main axis, with equal space around them.
space-evenly: Items are evenly distributed along the main axis with equal space around them, including before the first and after the last item.

<br>
<big>align-items:</big>

This property aligns flex items along the cross axis of the flex container.
Values include:
flex-start: Items are aligned to the start of the cross axis.
flex-end: Items are aligned to the end of the cross axis.
center: Items are centered along the cross axis.
baseline: Items are aligned such that their baselines align.
stretch: Items are stretched to fill the container along the cross axis.

<br>
<big>align-content:</big>

This property aligns flex lines within the flex container when there is extra space on the cross axis.
Values include:
flex-start: Lines are packed toward the start of the container.
flex-end: Lines are packed toward the end of the container.
center: Lines are centered in the container.
space-between: Lines are evenly distributed with equal space between them.
space-around: Lines are evenly distributed with equal space around them.
stretch: Lines are stretched to fill the container.

<br>
<big>
flex-direction:
</big>
This property sets the direction of the main axis.
Values include:
row: Main axis is horizontal, starting from the left and extending towards the right.
row-reverse: Main axis is horizontal, starting from the right and extending towards the left.
column: Main axis is vertical, starting from the top and extending towards the bottom.
column-reverse: Main axis is vertical, starting from the bottom and extending towards the top.

<br>
<big>flex-wrap:</big>

This property determines whether flex items are forced onto a single line or can wrap onto multiple lines.
Values include:
nowrap: All flex items are forced onto a single line.
wrap: Flex items wrap onto multiple lines if needed.
wrap-reverse: Flex items wrap onto multiple lines in reverse order if needed.

<Br>

Question.3:-
<br>
Answer:-
<br>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex -box in css</title>
    <style>
     *{
        margin: 0;
        padding: 0;
     }
        .body{
           height:100vh;
           width: 100vw;
            display: flex;
            justify-content: center;
            align-items:center;
        }
      #box{
            height: 100px;
            width:100px;
            background-color:green;
            
        }
    </style>
</head>
<body>
    <div class="body">
         <div id="box">
      
    </div>
</div>
   
</body>
</html>
<br>
Question.4:- A Client of yours wants to add a pricig section on their website to showcase their newly introduced Premium Plans.
<br>
Answers:- 
<Br>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Plans</title>
   <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link rel="stylesheet" href="stylesheet.css">
   
</head>
<body><section class="pricing-section">
    <div class="card-1">
         <h1 class="plan-name">Free Plan</h1>
            <p class="plan-for">for personal</p>
<p class="price">$0</p>       
 <p class="features"><i class="fa-solid fa-circle-check"></i> 1 Users</p>
 <p class="features"><i class="fa-solid fa-circle-check"></i> 4 website</p>
 <p class="features"><i class="fa-solid fa-circle-check"></i> Responsive Website</p>
 <p class="features"><i class="fa-solid fa-circle-check"></i> Free SSL</p>  
         
         <div class="subscribe-button"><button class="subscribe-now">Subscribe</button></div>

    </div>

    <!-- card 2 -->
    <div class="card-2"> 
        <h1 class="plan-name">Basic Plan</h1>
        <p class="plan-for">for Small Buisnesss</p>
<p class="price">$29</p>       
<p class="features"><i class="fa-solid fa-circle-check"></i> 4 Users</p>
<p class="features"><i class="fa-solid fa-circle-check"></i> 10 Web mails</p>
<p class="features"><i class="fa-solid fa-circle-check"></i> Responsive Website</p>
<p class="features"><i class="fa-solid fa-circle-check"></i> Free SSL</p>  
     
            <div class="subscribe-button">
                <button class="subscribe-now  dark-btn">Subscribe</button>
            </div>
    </div>

    <!-- card 3 -->
    <div class="card-3"> <h1 class="plan-name">Pro Plan</h1>
        <p class="plan-for">for enterprise</p>
<p class="price">$49</p>       
<p class="features"><i class="fa-solid fa-circle-check"></i> Unlimited Users</p>
<p class="features"><i class="fa-solid fa-circle-check"></i> Unlimited Web mails</p>
<p class="features"><i class="fa-solid fa-circle-check"></i> Responsive Website</p>
<p class="features"><i class="fa-solid fa-circle-check"></i> Free SSL + SEO</p>  
     
            <div class="subscribe-button">
                <button class="subscribe-now">Subscribe</button>
            </div></div>


</section>
     
</body>
</html>

<br>
<br>
Style {
body,p,h1,h2,h3 {
 margin:0;
    padding: 0;
    
}

body{
    height: 100vh;
    width: 100vw;
    display: flex;
    justify-content: center;
    align-items:center;
}
.pricing-section{
    width: 80vw; 
height: 427px;
margin-top: 25px;
margin-left: -8px;
padding: 32px, 48px, 32px, 48px;
background-color: #F4F2FD;
display: flex;
align-items: center;
justify-content: space-evenly;

}


/* card 1 */
.card-1{
    height:300px;
    width:220px;
   border-radius:8px;
   padding: 35px;
  gap: 20px;
  color: #202842;
   background-color: white;
}
.subscribe-button{
    width: 100%;
    display: flex;
    justify-content: center;
    margin-top:20px;;
    border-radius: 24px;
    font-size: 20px;
    border-color:transparent;
    height: 40px;
    width: 160px;  
}
.price{
    font-size:200%;
    font-weight: bold;
    margin:20px 0px 20px;
}
.plan-name{
    font-size: 30px;
}

        /* card-2 */

.card-2{
    height:350px;
    width: 220px;
    border-radius:4%;
    background-color:#202842;
    padding: 40px;
    color:white;
    /* display: flex; */
    
}
.subscribe-now {
    background-color:#202842 ;
    color:white
}
.dark-btn{
    background-color: white;
    color:#202842;
    align-self: flex-end;
}
/* card-3 */

.card-3{
    height: 300px;
    width: 220px;
    border-radius:8px;
    padding:32px;
    background-color: #FFFFFF;
   color: #202842;
    }
    }
