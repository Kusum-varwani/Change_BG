# Change_BG
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Change_BG</title>
  
    <style>
        *{
            padding:0px;
            margin: 0px;
            box-sizing: border-box;
        }
        #body{
            text-align: center;
            background-color:white;
            
        }
        button{
            margin-top:30%;
            font-size: 20px;
            
        }
    </style>
</head>
<body id="body">
    <button id="btn">change background color</button>
</body>
<script>

        var  r , g , b ;
        
        var body = document.getElementById ('body');

        var btn = document.getElementById  ('btn') ;


        btn.addEventListener('click',

            function() {

                do{
                    r = Math.round(Math.random()*1000);

                    g = Math.round(Math.random()*1000);

                    b = Math.round(Math.random()*1000);

                } 
                while((r > 255) || (g > 255) || (b > 255))
                
                body.style.backgroundColor = `rgb(${r},${g},${b})`;
            }
        )

</script>
</html>
