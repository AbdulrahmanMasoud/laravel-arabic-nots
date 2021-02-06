# Commands

``php artisan serv``

دي عشان اشغل المشروع بتاعي علي اللوكل هوست 

## Make New Controller

``php artisan make:controller ControlerName``

ده عشان ينشئ لي كنترولر جديد ولو عايز ينشئ لي كنترولر جديد مع الدوال اللي بستخدمها هكتب الامر ده

``php artisan make:controller ControlerName -r``

## Make New Model

``php artisan make:model ModelName -m``

ده بيعملي مودل جديد ولما انا ضيفت ال `-ام` بيعملي المايجريشن بتاعتي 

طيب لو كتبت كده

``php artisan make:model ModelName -a``

كده انا بقوله اعملي المودل و اعملي الميججريشن واعملي كنترولر كمان


## Migrations

``php artisan migrate``

دي عشان تنشئ الداتابيز بتاعتي اللي انا عملتها في الميجريشن

-----

# Routing

```Route::get('/path',[ControllerName::class,'method']);```

الراوت ده انا بعمله من خلال ان انا بكتي راوت وبعدين احدد الميثود اللي هيستخدمه سواء `جيت` او `بوست` او `بوت` او `دليت`
اللي هي دي

```Route::get();``` 
```Route::post();```
```Route::put();```
```Route::delete();```

وبعد كده بحدد المسار اللي هدخل عليه 

```Route::get('login');``` 

 وبعد كده انا بحددله الكنترولر اللي هيستخدمه اول اما يدخل علي المسار اللي انا حددته واحدد للكنترولر اي داله هيستخدمها في المسار ده
 ```Route::get('login',[LoginController::class,'userLogin']);```

يبقا هنا انا قولتله الراوت بتاعك نوعه `جيت` و المسار اللي هتدخل عليه اسمه `لوجين`
و الكنترولر اللي هتستخدمه اسمه `لوجين كنترولر` ونوعه كلاس
و الدله اللي هتستخدمها من الكنترولر ده اللي اسمها `يوزر لوجين`

```Route::apiResource('posts',[PostController::class]);```

هنا انا عملت روت جديد بس مش واخد جيت ولا بوست ولا اي حاجه من الحاجات دي عشان الروت انا محدده هيعمل كل الميثودث اللي  موجوده ف الكنترولر بتاع البوست  

-----
## Passing Data In Route

```Route::get('/user/{id}',[ControllerName::class,'method']);```





