---
layout: post
lang: vi
ref: jev-vs-laya
title: "jev hay laya: chọn mô hình quyết định cho doanh nghiệp"
description: Hai mô hình AI chỉ chọn trong những đáp án bạn cho phép. Bên nào thắng phụ thuộc vào thứ doanh nghiệp đã ghi lại.
permalink: /bai-viet/jev-va-laya/
---

Tháng 9/2026, TypeSafe AI ra mắt **Jev**. Ba ngày sau, Convai tung ra **Laya**, miễn phí và mã nguồn mở. Kênh Under the Hood AI đã so sánh hai mô hình trong [một video ngắn](https://www.youtube.com/shorts/4Q_YSgS2zMQ). Bài này tóm lại những gì video cho thấy, và điều người điều hành nên rút ra.

## mô hình quyết định là gì

Jev và Laya không phải chatbot. Chúng không viết câu nào. Bạn đưa vào một đoạn văn bản, ví dụ một email, kèm danh sách đáp án chấp nhận được ("lừa đảo" hay "an toàn", điểm từ 1 đến 5, có hay không). Mô hình trả về xác suất cho từng đáp án, và chỉ vậy.

Loại mô hình này làm những quyết định nhỏ, nhanh, lặp lại hàng nghìn lần trong một ứng dụng: chuyển email về đúng phòng ban, chặn nội dung không an toàn, giúp AI agent chọn bước tiếp theo.

## hộp đen và hộp kính

- **Jev là hộp đen.** TypeSafe chưa công bố cách mô hình hoạt động. Bạn gọi qua API và trả tiền theo lượng dùng.
- **Laya là hộp kính.** Trọng số, mã nguồn và tài liệu mô hình đều công khai theo giấy phép Apache 2.0. Mô hình dựa trên ModernBERT, nặng dưới 1 GB, chạy được trên laptop.

## số liệu trong video

| | Laya | Jev |
| --- | --- | --- |
| Tốc độ | khoảng 40 ms, chạy trên máy riêng | khoảng 240 ms, gọi qua internet |
| Chi phí | miễn phí, dữ liệu không rời máy | tính theo token, chạy trên cloud của TypeSafe |
| Dùng ngay, chưa huấn luyện | 36,2% | 72,7% |
| Sau khi luyện với 1.200 ví dụ có nhãn | 76,6% | |
| Khi có 77 đáp án để chọn | khoảng một nửa Jev | |

Video cũng lưu ý hai điểm. So tốc độ như vậy là không công bằng, vì Jev mất thêm thời gian đi qua mạng. Và 1.200 ví dụ dùng để luyện Laya lấy từ chính bộ đề dùng để chấm điểm.

Chi tiết đáng chú ý nhất: khi gặp văn bản tiếng Khmer, một hệ chữ nó không đọc được, Laya sai cả 100 câu mà vẫn tự tin 95%.

## điều lãnh đạo nên rút ra

**1. Bên thắng là bên có dữ liệu gán nhãn.** Laya chỉ vượt Jev sau khi được luyện bằng ví dụ có nhãn. Nhãn ở đây chính là tri thức tổ chức: email này thuộc phòng nào, yêu cầu kia là khiếu nại hay hỏi giá. Doanh nghiệp đã ghi lại những quyết định đó thì có lựa chọn rẻ hơn, nhanh hơn và giữ dữ liệu trong nhà. Doanh nghiệp chưa ghi lại thì phải trả tiền cho hộp đen.

**2. "Không thể hallucinate" không có nghĩa là đúng.** Cả hai công ty đều quảng cáo như vậy. Mô hình không bịa ra đáp án ngoài danh sách, nhưng vẫn chọn sai được, và có thể chọn sai một cách rất tự tin.

**3. Thử trên dữ liệu của mình trước khi tin con số của người khác.** Một mô hình đạt 77% trên bộ đề nó đã luyện chưa chắc giữ được mức đó với email của công ty bạn.

**4. Riêng tư là một lý do thật.** Với dữ liệu khách hàng hoặc hợp đồng, một mô hình chạy trong hạ tầng của mình có thể quan trọng hơn vài điểm phần trăm chính xác.

## chọn bên nào

Theo gợi ý của video:

- **Jev** khi bạn chưa có dữ liệu gán nhãn và cần chọn trong nhiều đáp án.
- **Laya** khi bạn có dữ liệu gán nhãn, cần tốc độ hoặc riêng tư, và có dưới 20 đáp án.

Câu chốt của video tóm gọn khác biệt này: Jev bán cho bạn câu trả lời, còn Laya trao cho bạn cái máy. Cái máy chỉ chạy tốt khi bạn có nguyên liệu để nạp vào nó.

*Nguồn: [Jev vs Laya Explained: TypeSafe AI vs the Open-Source Rival](https://www.youtube.com/shorts/4Q_YSgS2zMQ), kênh Under the Hood AI, 25/09/2026. Số liệu là của video, VietnamDX chưa tự kiểm chứng.*
