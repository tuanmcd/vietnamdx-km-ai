---
layout: post
date: 2026-10-29 14:00:00 +0700
lang: vi
ref: ai-at-the-centre
title: "đặt AI vào trung tâm: bài học từ người phụ trách claude code"
description: Anthropic tăng 8 lần lượng code mỗi kỹ sư bằng cách đặt AI vào giữa mọi quy trình, rồi gỡ từng nút thắt một. Lãnh đạo doanh nghiệp rút ra được gì.
permalink: /bai-viet/ai-o-trung-tam/
---

Trong một buổi trò chuyện với Mark, người dẫn chương trình bên AMD, Boris, người tạo ra và phụ trách Claude Code ở Anthropic, kể cách công ty anh làm việc khi AI đã nằm trong mọi quy trình. Bài này tóm lại [video 34 phút](https://www.youtube.com/watch?v=c4kYurm0hD8) và chọn ra những điểm chạm tới việc của người điều hành.

## máy tính ở góc phòng

Boris nhắc một bài trên Harvard Business Review từ thập niên 90, đặt câu hỏi vì sao có máy tính rồi mà năng suất không tăng. Câu trả lời là có hai kiểu công ty:

- **Kiểu thứ nhất** đặt máy tính ở một góc văn phòng, còn giấy bút và tủ hồ sơ vẫn giữ nguyên. Năng suất không đổi.
- **Kiểu thứ hai** bỏ tủ hồ sơ, đặt máy tính vào giữa mọi quy trình. Đó là những công ty thấy năng suất tăng thật.

Theo Boris, AI bây giờ cũng vậy. Những công ty dùng Claude thành công nhất là những nơi đặt nó vào trung tâm, không phải để bên cạnh.

## nhân viên mới hỏi AI, không hỏi wiki

Ví dụ của Boris là ngày đầu đi làm ở Anthropic. Ở hầu hết công ty, muốn biết địa chỉ văn phòng, cách xin quyền vào kho code hay cách nộp báo cáo công tác phí, bạn sẽ tra wiki hoặc hỏi đồng nghiệp. Ở Anthropic, bạn hỏi Claude.

Sau đó Claude tiếp tục có mặt trong mọi việc: viết code, review code, kiểm tra bảo mật, tổng hợp phản hồi người dùng, phân loại sự cố, nghĩ ý tưởng sản phẩm. Không chỉ ở khối kỹ thuật mà cả sản phẩm, thiết kế, marketing và kinh doanh.

Điều Boris không nói ra nhưng lãnh đạo nên thấy: Claude trả lời được câu hỏi của nhân viên mới chỉ vì những câu trả lời đó **đã được ghi lại ở đâu đó**. Đặt AI vào trung tâm là đặt tri thức của tổ chức vào trung tâm. Phần "bỏ tủ hồ sơ" của thời nay là đưa quy trình, chính sách và kinh nghiệm ra khỏi email và đầu người, vào nơi AI đọc được.

## gỡ từng nút thắt một

Từ đầu năm, lượng code mỗi kỹ sư ở Anthropic tăng 8 lần. Theo Boris, các khách hàng lớn đang thấy mức tăng 50 đến 150%, trong khi bình thường một công ty chỉ cải thiện vài phần trăm mỗi năm.

Cách làm không có gì bí ẩn: tìm nút thắt lớn nhất, giao cho AI, rồi tìm nút thắt tiếp theo. Đầu tiên là viết code. Khi code nhanh hơn thì review thành nút thắt, và cũng giao cho AI. Rồi tới tài liệu bán hàng. Cứ thế từng bước.

Khi kỹ thuật không còn là nút thắt, nút thắt chuyển sang **tốc độ nghĩ ra ý tưởng tốt và đưa ra thị trường an toàn**.

## từ một agent tới hàng nghìn agent

Boris mô tả các bậc mà doanh nghiệp đi qua:

| bậc | cách làm việc |
| --- | --- |
| 1 | mỗi kỹ sư chạy một agent, vẫn làm từng việc một |
| 2 | khoảng 10 agent, chuyển qua lại giữa các phiên |
| 3 | hàng chục tới hàng trăm agent, agent tự giao việc cho agent con |
| 4 | hàng nghìn agent, AI tự điều phối cả đội cho việc lớn |

Theo anh, phần lớn doanh nghiệp đang ở giữa bậc 1 và 2, còn Anthropic trung bình ở bậc 3. Ví dụ bậc 4 anh kể: Stripe chuyển một khối code Scala sang Java trong bốn ngày thay vì vài tháng.

## ROI: đừng chỉ nhìn chữ I

Đây là phần đáng đọc nhất cho lãnh đạo. Nhiều công ty tính ROI của AI bằng cách cắt chi phí: dùng model rẻ hơn, giảm mức suy luận. Boris nói việc đó nên làm, nhưng **phần quan trọng hơn là chữ R**, tức lợi ích thu về.

Muốn tăng R thì phải để mọi người thử nghiệm. Ý tưởng hay nhất thường không đến từ kỹ sư giỏi nhất mà từ một người mới ra trường, hoặc một nhân viên marketing ở góc nào đó trong công ty. Khi một cách dùng đã chứng minh hiệu quả, lúc đó mới tối ưu chi phí. Bỏ qua bước thử nghiệm thì không bao giờ tìm ra cơ hội.

Mark kể thêm một ví dụ từ AMD: một lỗi chip mà cả nhóm kỹ sư mất nhiều tuần chưa giải được, một kỹ sư trẻ dùng agent giải xong. Chuyện đó thuyết phục các kỹ sư lâu năm hơn mọi bài thuyết trình.

## việc của người lãnh đạo

Boris tóm vai trò của mình trong hai việc:

1. **Tạo không gian an toàn để thử.** Không ai bị đánh giá kém vì thử một ý tưởng mới. Nếu lãnh đạo không chủ động tạo không gian, mọi người sẽ tiếp tục làm theo cách cũ.
2. **Cho mọi người bối cảnh.** Bối cảnh kinh doanh, bối cảnh sản phẩm, để họ tự ra quyết định tốt hơn.

Việc thứ hai cũng là việc của AI. Boris nói khi model giỏi lên, anh làm việc với nó như với một kỹ sư lâu năm: tin, cho bối cảnh, cho mục tiêu, rồi kiểm tra định kỳ. Bối cảnh ấy phải nằm ở đâu đó để trao được, cho người lẫn cho máy.

## đo bằng gì, và tin đến đâu

- **Eval và cảm nhận.** Với quy trình lặp lại hàng nghìn lần, cần bộ đánh giá (eval) để biết model mới có tốt hơn không. Với những thứ khác, cảm nhận của người dùng là đủ, vì viết eval cũng tốn công.
- **Bỏ bấm "đồng ý" liên tục.** Khi agent hỏi xác nhận quá nhiều, người ta thôi đọc và bấm đồng ý cho xong. Anthropic chuyển việc duyệt sang một bộ phân loại tự động, kiểm chứng qua eval và kiểm thử xâm nhập, và thấy cách này an toàn hơn.

## sáu tháng tới

Boris không đoán hai ba năm, chỉ đoán sáu tháng: agent chạy lâu hơn, mỗi người chạy nhiều agent hơn, ít phải sửa hướng hơn. Chạy agent nhiều ngày liền sẽ thành chuyện bình thường, và có thể bắt đầu thấy cả sản phẩm, cả startup do Claude dựng.

## với doanh nghiệp việt nam

Ba câu hỏi đáng mang về cuộc họp ban điều hành:

- AI của công ty mình đang ở góc phòng hay ở giữa quy trình?
- Nhân viên mới hỏi AI thì nó có câu trả lời đúng không, và câu trả lời đó lấy từ đâu?
- Mình đang đo AI bằng chi phí cắt được, hay bằng những việc mới làm được?

*Nguồn: phỏng vấn Boris (Anthropic) trong chương trình của AMD, được đăng lại trên kênh hyperfixation on AI với tiêu đề [Stop Prompting — Head of Claude Code Uses Opus 5.5 + Graphs + Harness](https://www.youtube.com/watch?v=c4kYurm0hD8), 22/10/2026. Lưu ý: tiêu đề và mô tả của bản đăng lại nhắc tới "graph", "harness" và bộ nhớ, nhưng buổi trò chuyện không bàn những chủ đề đó. Số liệu là lời người được phỏng vấn, VietnamDX chưa tự kiểm chứng.*
