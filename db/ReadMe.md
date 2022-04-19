# Câu hỏi về DB:

## ACID Property:
Atomicity (Tính nguyên tử): All or Nothing Transactions
`Tất cả các hành động của một transaction cần được thực hiện thành công hoặc ngược lại nếu có một hành động không được thực hiện thì sẽ không có bất cứ hành động nào khác được thực hiện thành công.`

Consistency (Tính nhất quán): Guarantees Committed Transaction State
`Một giao dịch không bao giờ được thông qua khi cơ sở dữ liệu vẫn trong trạng thái dở dang. Tính chất này có nghĩa hoặc tạo ra 1 trạng thái mới hoặc rollback tất cả các xử lý để về trạng thái ban đầu.`

Isolation (Tính cô lập): Transactions are Independent
`Đảm bảo 2 hoặc nhiều giao dịch tách rời không trộn lẫn nhau cho đến khi chúng kết thúc. VD: Khi 1 người rút tiền đồng thời 1 người chuyển tiền vào cùng 1 tài khoản.`

Durability (Tính bền vững): Committed Data is Never Lost
`Khi transaction được diễn ra thành công hay thất bại hay dù có bất kỳ sự cố nào diễn ra với database (mất điện, server tràn bộ nhớ...) thì dữ liệu luôn được khôi phục về trạng thái trước khi có sự cố.`