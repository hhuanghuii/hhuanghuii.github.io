# hhuanghuii.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Document</title>

    <style>

        .out {

            position: absolute;

            width: 80px;

            height: 30px;

            background-color: gray;

            border-radius: 40px;

            transform: all 3s linear 0s;

        }

        .insert {

            position: relative;

            margin: 0px 0 0 .5px;

            width: 30px;

            height: 30px;

            background-color: #fff;

            border-radius: 50%;

        }

    </style>

    <script>

        window.onload = function (params) {

            var out = document.querySelector('.out')

            var insert = document.querySelector('.insert')

            var nu = 0;

            out.onclick = function (params) {

                if (nu == 0) {

                    insert.style.left = '49px'

                    document.body.style.backgroundColor = '#000'

                    nu = 1;

                } else {

                    insert.style.left = '0px'

                    document.body.style.backgroundColor = '#fff'

                    nu = 0;

                }

            }

        }

    </script>

</head>

<body>

    <div class="out">

        <div class="insert" id="insert"></div>

    </div>

</body>

</html>

