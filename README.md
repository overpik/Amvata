# Amvata 
***

## API : User Register
Method : POST

Link : "/xxxx"

Headers : 
```json
{
    "Content-Type": "application/json",
    "token":"xxxxxxxxxxxxxxxxx"
}
```

Request Parameter :
```json
{
    "phone": "095xxxxxxx",
    "email": "xxxxx@gmail.com",
    "password": "xxxx1234",
    "comfirm_password": "xxxx1234",
    "firstname": "firstname",
    "lastname": "lastname",
    "receive_news": "Y",
    "coupon": "Y",

}
```

Request Description :

| Name  | Type | Required | Description |
|---|---|---|---|
| phone  | number(10)  | true | เบอร์โทรศัพท์ |
| email  | string(50)  | true | อีเมล ต้องอยู่ในรูปแบบที่ถูกต้อง ตัวอย่าง. xxxxx@gmail.com |
| password  | string(8-16)  | true | รหัสผ่าน ต้องใส่ทั้งตัวเลขและตัวอักษร อย่างน้อย 8 ตัว|
| comfirm_password  | string(8-16)  | true | ยืนยันรหัสผ่าน ต้องใส่ทั้งตัวเลขและตัวอักษร อย่างน้อย 8 ตัว |
| firstname  | string(2-50)  | true | ชื่อ |
| lastname  | string(2-50)  | true | นามสกุล |
| receive_news | char(1)  | true | Y = รับข่าวสารและโปรโมชั่น, N = ไม่รับข่าวสารและโปรโมชั่น |
| coupon | char(1)  | true | Y = แจกคูปอง, N = ไม่แจกคูปอง |

Response Parameter :
```json
{
    "success": true,
    "message": "",
    "user_id": "xxxxx"
}
```
