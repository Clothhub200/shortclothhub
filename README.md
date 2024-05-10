<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        *{
            box-sizing:border-box;
        }
        :root{
              width:100vw;
              height:100vh;
        }
        body{
             display:flex;
             flex-direction: column;
             box-sizing:border-box;
        }
        .container{
             position:relative;
             width:fit-content;
             height:fit-content;
             box-shadow: 10px 5px 20px ;
             border-radius: 30px;
             display:flex
            
        }
        img{
            width:400px;
            height:400px;
            
            
        }
        .color{
             background:rgb(255, 25, 0);
             position:absolute;
             top:0;
             left:0;
             width:95%;
             height:95%;
             mix-blend-mode:multiply;
        }
        .txt{
              position:absolute;
              z-index:10;
              text-align:center;
              top:30%;
              left:63%;
              font-size:30px;
            
        }
        option{
              width:auto;
              height:auto;
        }
        #txt-input{
               width:20%;
        }
        .kit{
              width:100%;
              box-shadow:10px 5px 25px rgba(0,0,0,0.2);
              border-radius:20px;
              display:flex;
              flex-wrap: wrap;
              gap:20px;
              padding:20px;
        }
        .kit:hover{
              cursor:pointer;
        }
        .logo{
             position:absolute;
             top:30%;
             right:65%;
             mix-blend-mode: multiply;
        }
        .grd{
               display:flex;
               gap:50px;
               width:100%;
        }
        .txt-box{
               display:flex;
               gap:20px;
               width:100%;
        }
        .main{
              display:flex;
              justify-content: space-around;
              width:100%;
              height:100%;
              
        }
        .box2{
               width:100%;
               padding:20px;
               border-radius:30px;
               box-shadow:10px 5px 25px rgba(0,0,0,0.2);
               display:grid;
               grid-template-columns: 1fr 1fr 1fr 1fr 1fr   ;
               gap:0px;
        }
        .design2{
            position:absolute;
            mix-blend-mode: multiply;
            z-index:10;
            top:40%;
            left:62%;
            
        }
        .logo5{
            position:absolute;
            top:45%;
            right:66%;
            mix-blend-mode: multiply;
        }
        .box3{
            width:100%;
            padding:20px;
            border-radius:30px;
            box-shadow:10px 5px 25px rgba(0,0,0,0.2);
            display:grid;
            grid-template-columns: 1fr 1fr 1fr 1fr 1fr   ;
            gap:0px;
     }
    </style>
</head>
<body>
    
<div style="display:flex;">
<div class="main">
<div >
 <div class="container">
    <img src="https://i.pinimg.com/originals/78/fe/ab/78feabcb5e6fa78f4f27c5c70eb11bb7.png" style="width:750px; height:500px;" />
    <div class="color"></div>
    <div class="txt"> </div>
    <div class="logo">
         <img  src="https://i.pinimg.com/564x/c4/57/91/c457912ca5ec78b64beb6f276d39a899.jpg" style="width:120px; height:120px; position:absolute; right:100px; top:190px; "/>
    </div>
    <div class="logo5">
        <img  src="" style="width:100px; height:80px;"/>
   </div>
    <div class="design2">
        <img  src="https://i.pinimg.com/564x/fd/d4/55/fdd45584514731a5884b3708369a12e8.jpg" style="width:120px; height: 120px; border-radius:300px; position:absolute; left:110px; top: 140px;"/>
    </div>
 </div style="width:100%;">
 <div class="grd">
    <div>
     <h1>Color Pallete</h1>
     <input type="color" value="#ff0000" id="clr">
    </div>
    <div>
     <h1>Text Box</h1>
    <div class="txt-box">
       <input type="text" value="" id="txt-input" style="width:80%; ">
        <input type="color" value="" id="clr2" >
    </div>
    </div>
</div>
</div>
<div style="display:flex; flex-direction:column; gap:70px;">
<div class="kit">
     
</div>
<div class="box2">
     
</div>
<div class="box3">
     
</div>
</div>
</div>
 <script>
       const imgArr=['https://i.pinimg.com/564x/c4/57/91/c457912ca5ec78b64beb6f276d39a899.jpg',"https://i.pinimg.com/564x/e7/65/04/e7650458fe434cd647eafb289a569fe2.jpg"];
       const designArr = ['https://i.pinimg.com/564x/fd/d4/55/fdd45584514731a5884b3708369a12e8.jpg','https://i.pinimg.com/564x/52/a2/83/52a28335ba769eb84e4853ada1ec618f.jpg','https://i.pinimg.com/564x/1f/3c/39/1f3c394be71582bff9f80be042461178.jpg',]
       const design2Arr = ['data:image/png;base64,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']
       const clr = document.getElementById('clr');
       const kit = document.querySelector('.kit');
       const design =  document.querySelector('.box2');
       const design3 =  document.querySelector('.box3');
       const txt_select = document.querySelector('#txt-input');
       const tshirt = document.querySelector('.color');
       const txt_box = document.querySelector('.txt');
       const logo = document.querySelector('.logo img');
       const clr2 = document.getElementById('clr2');
       const design2 = document.querySelector('.design2 img');
       const design4 = document.querySelector('.logo5 img');
       const fileInput = document.querySelector('.file-input');
       const logo5 = document.querySelector('.logo5 img');
       clr.addEventListener('input',(e)=>{
            tshirt.style.background=e.target.value;
       });
       clr2.addEventListener('input',(e)=>{
        txt_box.style.color=e.target.value;
   });
       txt_select.addEventListener('keyup',(e)=>{
            txt_box.innerHTML = e.target.value;
       });
       imgArr.forEach((ele,index)=>{
          kit.innerHTML += `<img src=${ele} class='logo2' style="width:70px; height:70px;"/>`;
          const kitChild = document.querySelectorAll('.kit .logo2');
          for(let i=0;i<kitChild.length;i++)
          {
             kitChild[i].addEventListener('click',()=>{
                 logo.src=`${imgArr[i]}`;
             })
          }
       });
       designArr.forEach((ele)=>{
         design.innerHTML += `<img src=${ele} class='logo3' style="width:50px; height:50px;"/>`;
         const kitChild = document.querySelectorAll('.box2 .logo3');
         for(let i=0;i<kitChild.length;i++)
         {
            kitChild[i].addEventListener('click',()=>{
                 design2.src=`${designArr[i]}`;
            })
         }
       })
       design2Arr.forEach((ele)=>{
        design3.innerHTML += `<img src=${ele} class='logo9' style="width:50px; height:50px;"/>`;
        const kitChild = document.querySelectorAll('.box3 .logo9');
        for(let i=0;i<kitChild.length;i++)
        {
           kitChild[i].addEventListener('click',()=>{
                design4.src=`${design2Arr[i]}`;
           })
        }
      })
       fileInput.addEventListener('input',(e)=>{
          logo5.src=e.target.value;
       });

 </script>
</body>
</html>
