# Boolean คือค่าความจริง มีแค่ 2 ค่าเท่านั้น:
True
False

## ใน Python เรามักได้ Boolean จากการเปรียบเทียบ เช่น
5 > 3      # True
5 < 3      # False
5 == 5     # True
5 != 5     # False

# เครื่องหมายที่ต้องรู้
>     มากกว่า
<     น้อยกว่า
>=    มากกว่าหรือเท่ากับ
<=    น้อยกว่าหรือเท่ากับ
==    เท่ากับ
!=    ไม่เท่ากับ


## ข้อควรระวังมาก:
x = 5

แปลว่า กำหนดค่า 5 ให้ x

แต่

x == 5

แปลว่า ตรวจว่า x เท่ากับ 5 หรือไม่


# ตัวดำเนินการ and / or / not
## 1. and
and จะเป็น True ก็ต่อเมื่อทั้งสองฝั่งเป็น True

True and True    # True
True and False   # False
False and True   # False
False and False  # False

ตัวอย่าง:

x = 10
x > 5 and x < 20

คิดแบบนี้:

x > 5   คือ True
x < 20  คือ True
True and True = True

ตอบ True

## 2. or
or จะเป็น True ถ้ามีอย่างน้อย 1 ฝั่งเป็น True

True or True     # True
True or False    # True
False or True    # True
False or False   # False

ตัวอย่าง:

x = 10
x < 5 or x > 8

คิดแบบนี้:

x < 5  คือ False
x > 8  คือ True
False or True = True

ตอบ True

## 3. not
not คือกลับค่าความจริง

not True     # False
not False    # True

ตัวอย่าง:

x = 10
not (x > 5)

คิดแบบนี้:

x > 5 คือ True
not True คือ False

ตอบ False


# important ผลเศษจะต้องมีเครื่องหมายตามตัวหาร (Divisor) เสมอ

รูปแบบ	       เครื่องหมายของผลลัพธ์	        ตัวอย่าง	       ผลลัพธ์ที่ได้
บวก % บวก	       บวก (ตาม b)	        3 % 2	                1
ลบ % บวก	       บวก (ตาม b)	        -3 % 2	                 1
บวก % ลบ	       ลบ (ตาม b)	        3 % -2	               -1
ลบ % ลบ	          ลบ (ตาม b)	        -3 % -2	                -1

'''

$$a \bmod b = a - b \left\lfloor \frac{a}{b} \right\rfloor$$

'''