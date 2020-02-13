# Amvata 
***

## API : API User Register
Method : POST

Link : "https://amvata.com/api-user-register-th"

Headers : 
```json
{
    "Content-Type": "application/json",
    "token": `$token`
}
```

Request Body Parameter :
```json
{
    "phone": "095xxxxxxx",
    "email": "xxxxx@gmail.com",
    "password": "xxxx1234",
    "firstname": "firstname",
    "lastname": "lastname",
    "receive_news": "Y",
    "coupon": "Y",
    "from": "ABK"
}
```

Request Description :

| Name  | Type | Required | Description |
|---|---|---|---|
| phone  | number(10)  | true | เบอร์โทรศัพท์ |
| email  | string(50)  | true | อีเมล ต้องอยู่ในรูปแบบที่ถูกต้อง ตัวอย่าง. xxxxx@gmail.com |
| password  | string(8-16)  | true | รหัสผ่าน ต้องใส่ทั้งตัวเลขและตัวอักษร อย่างน้อย 8 ตัว|
| firstname  | string(2-50)  | true | ชื่อ |
| lastname  | string(2-50)  | true | นามสกุล |
| receive_news | char(1)  | true | Y = รับข่าวสารและโปรโมชั่น, N = ไม่รับข่าวสารและโปรโมชั่น |
| coupon | char(1)  | true | Y = แจกคูปอง, N = ไม่แจกคูปอง |
| from | string(50)  | true | APK = ลงทะเบียนจากงาน APK, BS =ลงทะเบียนจากงาน BS |

Response Parameter :
```json
{
    "status": true,
    "message": "success",
    "user_id": "xxxxx"
}
```

Response Description :

| Name  | Type | Description |
|---|---|---|
| status  | boolean | API status success = true, error = false |
| message  | string |  show message status |
| user_id  | number | response when status = true|
