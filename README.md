# 01-flex_container--flex-direction--flex-wrap

```html

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

# 02-flexbox_alignments
```html


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
            height: 500px;
            
            /* Yatayda hizalama */
            /* justify-content: center; */
            /* justify-content: flex-start; */
            /* justify-content: flex-end; */

            
            /* Dikey hizalama */
            /* align-items: stretch; */
            /* align-items: flex-start; */
            /* align-items: flex-end; */


            /* Itemler arası boşluk */
            /* justify-content: space-around; */
            /* justify-content: space-between; */
            /* justify-content: space-evenly; */


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
    </div>

</body>
</html>

```

# 03-flex-item-alignments

```html


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
            display: flex;
            height: 500px;
            flex-direction: column;
            align-items: flex-end;

        }

        .item{
            background-color: #f7786b;
            padding: 30px;
            margin: 20px;
            color: #fff;
            font-size: 25px;
        }
        .item-1{
            align-self: flex-start;
            /* item-1 ögesini kutunun başına aldı */
        }
        .item-2{
            align-self: center;
            /* item-2 ögesini kutunun ortasına aldı */
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="item item-1">Item 1</div>
        <div class="item item-2">Item 2</div>
        <div class="item item-3">Item 3</div>
        <div class="item item-4">Item 4</div>
    </div>

</body>
</html>

```

# 04-flex-item-properties

```html


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
            display: flex;
            height: 500px;

        }

        .item{
            background-color: #f7786b;
            padding: 30px;
            margin: 20px;
            color: #fff;
            font-size: 25px;
        }
        .item-1{
            /* 2 Birimlik alan kapla */
            flex-grow: 2;
        }
        .item-2{
            /* 1 Birimlik alan kapla */
            flex-grow: 1;
        }
        .item-3{
            /* 200 px alan kapla */
            flex-basis: 200px;
            /* ekran küçülse bile küçülme */
            flex-shrink: 0;
        }
        .item-4{
            /* 1 Birimlik alan kapla */
            flex-grow: 1;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="item item-1">Item 1</div>
        <div class="item item-2">Item 2</div>
        <div class="item item-3">Item 3</div>
        <div class="item item-4">Item 4</div>
    </div>

</body>
</html>


```

# 05-flex-row-alignments

```html


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
            display: flex;
            height: 500px;

            /* İçerikler sığmazsa aşağı geçsinler */
            flex-wrap: wrap;
            
            /* İçerikler arasındaki boşluk (margin) */
            gap: 20px;

            /* İçerik hizalama */
            /* align-items: center; */
            align-content: center;
            /* align-content: flex-start; */
            /* align-content: flex-end; */
            /* align-content: space-around; */
            /* align-content: space-between; */
            /* align-content: space-evenly; */


        }

        .item{
            background-color: #f7786b;
            padding: 30px;
            /* margin: 20px; */
            color: #fff;
            font-size: 25px;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="item item-1">Item 1</div>
        <div class="item item-2">Item 2</div>
        <div class="item item-3">Item 3</div>
    </div>

</body>
</html>

```

# 06-flex-margin

```html


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
            display: flex;
            height: 500px;
        }

        .item{
            background-color: #f7786b;
            padding: 30px;
            margin: 20px;
            color: #fff;
            font-size: 25px;

            /* İçerikleri otomatik olarak yaslar */
            /* margin: auto; */
            /* margin-top: auto; */
            /* margin-bottom: auto; */
            /* margin-right: auto; */
            /* margin-left: auto; */
        }

        .item-1{
            /* item-1 soldan ve yukarıdan kendini ittirir */
            margin-left: auto;
            margin-top: auto;
        }
        .item-2{
            /* item-2 sağdan ve yukarıdan kendini ittirir */
            margin-right: auto;
            margin-top: auto;
        }
    </style>
</head>
<body>

    <div class="container">
        <div class="item item-1">Item 1</div>
        <div class="item item-2">Item 2</div>
    </div>

</body>
</html>

```
