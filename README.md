<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Logic Form in HTML and CSS</title>
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
    <style>
        .{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        }
        body{
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background: url(https://images.unsplash.com/photo-1617957772002-57adde1156fa?fm=jpg&q=60&w=3000&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxleHBsb3JlLWZlZWR8Mnx8fGVufDB8fHx8fA%3D%3D) no-repeat;
            background-size: cover;
            background-position: center;
        }
        .wrapper{
            width: 420px;
            background-color: transparent;
            border: 2px solid rgba(255, 255, 255, .2);
            backdrop-filter: blur(100px);
            box-shadow: 0 0 10px rgba(0, 0, 0, .1);
            color: #fff;
            border-radius: 10px;
            padding: 30px 40px;
        }
        .wrapper h1{
            font-size: 36px;
            text-align: center;
        }
        .wrapper .input-box{
            position: relative;
            width: 100%;
            height: 50px; 
            margin: 30px 0;
        }
        .input-box input{
            width: 83%;
            height: 40%;
            background: transparent;
            border: none;
            outline: none;
            border: 2px solid rgba(216, 208, 208, 0.2);
            border-radius: 40px;
            font-size: 16px;
            color: #fff;
            padding: 20px 45px 20px 20px    ;
        }
        .input-box input::placeholder{
            color: #fff;
        }
        .input-box i{
            position: absolute;
            right: 20px;
            top: 65%;
            transform: translateY(-50%);
            font-size: 20px;
        }
        .wrapper .remember-forgot{
            display: flex;
            justify-content: space-between;
            font-size: 14.5px;
            margin: -15px 0 15px;
        }
        .remember-forgot label input{
            accent-color: #fff;
            margin-right: 3px;
        }
        .remember-forgot a{
            color: #fff;
            text-decoration: none;
        }
        .remember-forgot a:hower{
            text-decoration: underline;
        }
        .wrapper .btn{
            width: 100%;
            height: 45px;
            background: #fff;
            border: none;
            outline: none;
            border-radius: 40px;
            box-shadow: 0 0 10px rgba(0, 0, 0, .1);
            cursor: pointer;
            font-size: 16px;
            color: #333;
            font-weight: 100;
        }
        .wrapper .register-link{
            font-size: 14.5px;
            text-align: center;
            margin: 20px 0 15px;
        }
        .register-link p a{
            color: #fff;
            text-decoration: none;
            font-weight: 600;
        }
        .register-link p a:hover{
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <div class="wrapper">
        <form action="">
            <h1>Login</h1>
            <div class="input-box">
                <input type="text" placeholder="Username" required>
                <i class='bx bxs-user'></i>
            </div>
            <div class="input-box">
                <input type="password" placeholder="Password" required>
                <i class='bx bxs-lock-alt' ></i>
            </div>
            <div class="remember-forgot">
                <label ><input type="checkbox" >Remember Me</label>
                <a href="#">Forgot Password</a>
            </div>
            <button type="submit" class="btn">login</button>
        </form>
        <div class="register-link">
            <p>Don't have an acount? <a href="#">Register</a></p>
        </div>
    </div>
</body>
</html>
