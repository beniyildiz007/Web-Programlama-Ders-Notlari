# html

```css

<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <style>
        .container{
            background-color: #034f84;
            padding: 15px;
            display: flex;

            /* Hizalama:↓↓ */
            /* flex-direction: row;
            flex-direction: column;
            flex-direction: row-reverse;
            flex-direction: column-reverse; */

            /* Varsayılan => nowrap */
            /* flex-wrap: nowrap; */
            /* flex-wrap: wrap; */
            /* flex-wrap: wrap-reverse; */


            /* Direction ve Wrap beraber kullanımı:↓↓ */
            /* flex-flow: row wrap; */
            /* flex-flow: row wrap-reverse; */
            /* flex-flow: column wrap; */
            /* flex-flow: column wrap-reverse; */



        }

        .item{
            background-color: #f7786b;
            padding: 30px;
            margin: 20px;
            color: #fff;
            font-size: 25px;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="item">Item 1</div>
        <div class="item">Item 2</div>
        <div class="item">Item 3</div>
        <div class="item">Item 4</div>
        <div class="item">Item 5</div>
    </div>

</body>
</html>

```
