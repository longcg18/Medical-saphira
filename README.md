# Saphira

## Quy trình làm việc
Để bắt đầu và hoàn thành một task, quy trình sẽ nên là như sau:
* Nhận task hoặc xem mình được assign task nào chưa.
* Cố gắng đọc kỹ phần mô tả và code đúng yêu cầu.
* Sau khi hoàn thành, tạo PR và mô tả rõ code mình đã làm thêm cái gì.
* Assign ít nhất 2 reviewer để ae vào check, nếu cả 2 cùng approve thì merge.

**Lưu ý** : 
* Khi bắt đầu code cho một task nào đó, mọi người phải tạo branch mới từ nhánh ***main*** với tên branch liên quan tới task của mình (Không được đặt tên chung chung kiểu như "*Fig bug*", "*Thêm chức năng*", ...)
* Từ nhánh mới tạo commit code dần vào nhánh đó (Thằng nào commit thẳng vào main phạt ***50k***)
* Thỉnh thoảng check xem nhánh main có gì mới không, nếu có thì nên merge về nhánh của mình tránh bị tụt hậu rồi lúc merge bị conflict
* Cố gắng code sáng sủa, dễ đọc. Nếu không tự tin có thể dùng thêm extension.
* Không khuyến khích "vạch lá tìm sâu".

## Hỗ trợ về phần mềm
* [Visual Studio Code](https://code.visualstudio.com/download)
* Extension Prettier (Tìm trên mục extension ở VS Code rồi tìm cách cài đặt, khi lưu file extension sẽ tự căn chỉnh code cho mình)
* [Github Desktop](https://desktop.github.com/)

## Dán PR từ repo gốc sang
* Repo nguồn: [Saphira](https://github.com/dwngh/saphira)
* Giải thích:
    * Ở repo nguồn, mỗi một PR sẽ ứng với một branch
    * Việc Dán PR từ repo gốc sang chính là đem code của branch ứng với PR đó sang repo mới
* Các bước:
    * Tạo branch tương ứng với branch ở PR được giao ở repo mới (VD: PR [#8](https://github.com/dwngh/saphira/pull/8) của repo cũ có branch tương ứng ```07-init-front-end```)
    * Kéo code từ branch trên ở repo cũ về máy, sau đó copy sang thư mục của repo mới (Lưu ý: Trừ folder ```node_modules```) 
        * VD: Kéo code từ [đây](https://github.com/dwngh/saphira/tree/07-init-front_end) về máy
    * Commit thay đổi vừa rồi vào branch tương ứng ở repo mới
    * Tạo PR ở repo mới, để cho nhanh ta có thể copy y hệt nội dung ở PR cũ sang PR mới
    * Sau đó add reviewer là ```dwngh``` và một người ngẫu nhiên nữa
    * Lướt xuống cuối, thay vì merge thông thường ta chọn **Squash and merge**
