---
marp: true
title: P4DS
paginate: true
theme: gaia
class: lead
backgroundColor: #fff
backgroundImage: url('https://marp.app/assets/hero-background.svg')
---


# P4DS

## Final Project
---

## Thông tin nhóm

**Nhóm 18**
Họ và tên: **Nguyễn Văn Hùng**
MSSV: **1712222**

---

# Chủ đề

### Tìm hiểu về giá thuê căn hộ tại TP HCM

---

1. Thu thâp dữ liệu

+ Data về giá thuê căn hộ được lấy từ [nhatot.vn](https://batdongsan.com.vn/cho-thue-can-ho-chung-cu-tp-hcm)

+ Crawl data bằng API của chotot:

---
```
https://gateway.chotot.com/v1/public/ad-listing?region_v2=13000&cg=1010&o=0&page=0&st=s&limit=20&w=1
```

```json
{
    "variant": 0,
    "total": 28448,
    "ads": [
        {
            "ad_id": 137757745,
            "list_id": 99684873,
            "list_time": 1670252210741,
            "subject": "Căn ...",
            "category": 1010,
            "category_name": "Căn hộ/Chung cư",
            "area": 103,
            "area_name": "Quận 8",
            "region": 13,
            "region_name": "Tp Hồ Chí Minh",
            "company_ad": true,
            "type": "s",
            "price": 550000000,
            "price_string": "550 triệu",
            "videos": [],
            "number_of_images": 5,
            "rooms": 1,
            ..
        }, ...
    ]
}
```

---

## 2. Khám phá dữ liệu

+ Kiểm tra số dòng cột
+ Ý nghĩa dòng, cột
+ Kiểm tra null
+ Kiểm tra lặp
+ Phân bố các cột numeric
+ Phân bố các cột category

---

## 3. Đặt câu hỏi

1. Giá thuê căn hộ ở các quận chênh lệch như thế nào?
   + **Ý nghĩa**: Có cái nhìn tổng quát về giá thuê nhà tại các quận, giá theo diện tích, theo số phòng, theo loại hình để có thể xem xét và đưa ra quyết định nên thuê ở đâu, các đặc điểm của căn hộ ra sao.

2. Các yếu tố ảnh hưởng tới giá thuê nhà?
   + **Ý nghĩa**: Để hiểu thêm về sự tương quan giữa giá thuê với các yếu tố khác như diện tích, số phòng, số nhà vệ sinh, vị trí, ...

3. Tìm một căn hộ phù hợp để thuê theo một số tiêu chí?
   + **Ý nghĩa**: thực tế chỉ là để tham khảo chọn phòng để thuê

---

## 4. Trả lời câu hỏi

+ Câu 1:

+ Câu 2:

+ Câu 3:

---

## 5. Tổng kết

+ Khó khăn

+ Cải thiện

+ Nguồn tham khảo