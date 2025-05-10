<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تسجيل الدخول | GitHub</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f6f8fa;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .login-container {
            background-color: white;
            border: 1px solid #e1e4e8;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
            width: 400px;
            padding: 40px;
            border-radius: 6px;
            text-align: center;
        }

        h2 {
            margin-bottom: 20px;
            font-size: 24px;
            font-weight: 600;
            color: #333;
        }

        .form-field {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border: 1px solid #d1d5da;
            border-radius: 4px;
            font-size: 16px;
            background-color: #f6f8fa;
        }

        .form-field:focus {
            outline: none;
            border-color: #0366d6;
            background-color: white;
        }

        .submit-btn {
            width: 100%;
            padding: 12px;
            background-color: #2c974b;
            color: white;
            font-size: 16px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
        }

        .submit-btn:hover {
            background-color: #236a36;
        }

        .google-login-btn {
            width: 100%;
            padding: 12px;
            background-color: #4285f4;
            color: white;
            font-size: 16px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            margin-top: 10px;
        }

        .google-login-btn:hover {
            background-color: #357ae8;
        }

        .forgot-password {
            font-size: 14px;
            color: #0366d6;
            text-decoration: none;
            margin-top: 10px;
        }

        .forgot-password:hover {
            text-decoration: underline;
        }

        .create-account {
            margin-top: 20px;
            font-size: 14px;
        }

        .create-account a {
            color: #0366d6;
            text-decoration: none;
        }

        .create-account a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>

    <div class="login-container">
        <h2>تسجيل الدخول إلى GitHub</h2>

        <!-- نموذج تسجيل الدخول باستخدام البريد الإلكتروني وكلمة المرور -->
        <input type="email" class="form-field" placeholder="البريد الإلكتروني" required>
        <input type="password" class="form-field" placeholder="كلمة المرور" required>

        <!-- زر لتسجيل الدخول باستخدام البريد الإلكتروني -->
        <button class="submit-btn">تسجيل الدخول</button>

        <!-- زر تسجيل الدخول باستخدام Google -->
        <button class="google-login-btn">تسجيل الدخول باستخدام Google</button>

        <!-- رابط "نسيت كلمة المرور؟" -->
        <a href="#" class="forgot-password">هل نسيت كلمة المرور؟</a>

        <!-- رابط "إنشاء حساب جديد" -->
        <div class="create-account">
            <p>لا تمتلك حسابًا؟ <a href="#">إنشاء حساب</a></p>
        </div>
    </div>

</body>
</html>
