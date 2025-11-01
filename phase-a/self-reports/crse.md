# SE358 - Báo cáo cá nhân

Trước đây, các dự án phần mềm em thực hiện đều xuất phát từ sở thích cá nhân nên không có kiến trúc, quy trình hay tài liệu đầy đủ. Nhằm tìm hiểu và làm quen với quy trình thực hiện một dự án phần mềm, em đã chọn đề tài liên quan đến Hệ thống Website Quản lý lớp học Online (từ đây sẽ gọi là Crse) để thực hiện trong dự án môn học Nhập môn Công nghệ Phần mềm. Dự án có quy mô nhỏ, với mục tiêu là tạo ra một nền tảng giúp học viên và giảng viên có thể trao đổi hoạt động học tập trực tuyến thay vì Messenger hay Zalo. Nhóm cũng tận dụng thời gian thực hiện dự án để làm quen với các khái niệm chuyên ngành và các công cụ hỗ trợ có liên quan.

Crse chỉ hỗ trợ tiếng Việt và nhắm đến đối tượng người dùng là học sinh, giáo viên và các cơ sở giáo dục trong nước. Nhóm có tham khảo các hệ thống hiện hành tương tự như Classroom hay Moodle và thiết kế hệ thống với các chức năng chính như xác thực và phân quyền người dùng, quản lý môn học, đăng tải tài liệu, nộp bài tập, tạo và làm bài thi, và forum thảo luận cho mỗi lớp học. Dù vậy do nguồn lực và thời gian có hạn nên hệ thống chỉ triển khai ở phạm vi một lớp học và chưa có các chức năng nâng cao như chấm điểm tự động.

Lộ trình thực hiện dự án song song với nội dung của bài giảng trên lớp, cụ thể:

- **Tuần 1-2:** Thu thập yêu cầu, thiết kế form khảo sát về thói quen
  học tập online ở nhà, trao đổi tài liệu qua các kênh liên lạc hiện
  hành, các bất cập của các hệ thống đó.
- **Tuần 3-4:** Nhóm bắt đầu mô hình hóa yêu cầu, làm ERD, làm
  Function List, User Story, thiết kế sơ đồ Use-case và đặc tả.
- **Tuần 5-6:** Vẽ các sơ đồ Sequence, Activity cho các Use-case. Vẽ
  sơ đồ trạng thái, sơ đồ miền cho dự án.
- **Tuần 7:** Lên thiết kế cho giao diện và các UI Components.
- **Tuần 8-10:** Lập trình Front-end và Back-end.
- **Tuần 11-12:** Kiểm thử hệ thống và sửa các bug được phát hiện.
- **Tuần 13:** Hoàn thiện báo cáo đồ án.

Thực tế, dự án gặp nhiều khó khăn để theo kịp lộ trình đã đề ra do các thành viên trong nhóm đều chưa thành thạo trong nhiều giai đoạn của quy trình, đặc biệt là phần vẽ Diagram. Nhóm phải liên tục trao đổi với giảng viên để được hỗ trợ. Ngoài ra, các thành viên trong team Backend phải dành thời gian để học JavaScript và tìm hiểu về NodeJS và ExpressJS. Nhóm cũng phân vân trong việc lựa chọn hệ quản trị cơ sở dữ liệu thích hợp cho dự án. Tuy nhiên, các chức năng chính và giao diện của hệ thống vẫn được hoàn thành và triển khai trước ngày báo cáo môn học.

Do quy mô nhỏ nên dự án không tốn chi phí để phát triển, nhóm đã sử dụng Free Plan trên Vercel để host Front-end và Render để host Back-end. Tuy nhiên, vì chính sách miễn phí của Render nên mỗi lần gửi request, server phải cần khoảng 1 phút để khởi động. Bên cạnh đó, nhóm còn sử dụng các công cụ miễn phí như GitHub để lưu source code và Figma để thiết kế giao diện.

Sản phẩm đạt được vài ưu điểm nổi bật như giao diện thân thiện, dễ làm quen và sử dụng. Các chức năng cơ bản của hệ thống như xác thực và phân quyền, đăng tải file, nộp bài tập được hoàn thành và hoạt động như yêu cầu. Thời gian phản hồi request, thời gian truy xuất từ hệ cơ sở dữ liệu cũng đáp ứng yêu cầu dưới 1 giây. Tuy nhiên, hệ thống vẫn tồn tại nhiều hạn chế, ví dụ như một vài form chưa có xác thực dữ liệu nhập vào; hệ thống xác thực chỉ mới sử dụng Google OAuth chứ chưa có tùy chọn đăng nhập bằng tài khoản và mật khẩu; giao diện chưa được tối ưu cho điện thoại.

Nhóm thực hiện dự án gồm 3 thành viên, được phân công rõ ràng: 1 người thiết kế giao diện và lập trình Front-end sử dụng Figma, thư viện React và TailwindCSS, 2 người lập trình Back-end sử dụng ExpressJS và NodeJS, cả nhóm tham gia thiết kế cơ sở dữ liệu MySQL và viết tài liệu, báo cáo bằng LaTeX thông qua Overleaf. Các nguồn tài liệu học tập gồm w3schools, freeCodeCamp, Youtube,\... Mã nguồn của dự án được lưu trên GitHub. Vì kinh nghiệm còn hạn chế nên nhóm đều sử dụng các nền tảng quen thuộc và công nghệ đơn giản.

Trong quá trình phát triển, dự án đã gặp một số rủi ro. Đặc biệt nhất là rủi ro về bảo mật khi nhóm chưa có kinh nghiệm trong việc xử lý các lỗ hổng dữ liệu. Ngoài ra, do sử dụng Free Plan của Render nên hệ thống mang đến trải nghiệm người dùng không được tốt do server chỉ có thể chịu được lượng request thấp và cần thời gian để khởi động. Hệ thống còn có nguy cơ bị quá tải khi lượng người dùng truy cập đồng thời cao.

Dự án có thể được xem là thành công ở mức độ môn học do đã có sản phẩm và demo chạy được với các chức năng cơ bản. Bộ tài liệu của dự án cũng được hoàn thành theo chuẩn của môn học và được giảng viên chấp nhận. Tuy nhiên, nếu xét đến mục tiêu ban đầu nhóm đề ra thì dự án chưa được xem là thành công trọn vẹn. Các chức năng như chấm điểm tự động hay giao diện mobile vẫn chưa được hoàn thiện đúng lộ trình. Nguyên nhân chính là việc quản lý tiến độ chưa chặt chẽ, một số thành viên không đảm bảo được thời gian làm việc, còn delay deadline. Dù vậy, trong tương lai, hệ thống vẫn tiếp tục được phát triển thêm và sửa lỗi để hoàn thiện hơn.

Crse chính là dự án đầu tiên trong lĩnh vực phần mềm của nhóm, vì thế, nhóm đã tiếp cận được rất nhiều kiến thức mới cũng như rút ra được nhiều kinh nghiệm quý báu. Trước đây, chúng em đã nghĩ phát triển phần mềm chỉ đơn giản là code, tuy nhiên, trong thực tế việc code chỉ chiếm khoảng 30% trong quy trình phát triển. Trước hết, việc xác định phạm vi dự án cũng như phân tích yêu cầu đóng vai trò rất quan trọng vì chúng là nền tảng cho dự án, giảm thiểu các rủi ro trong các giai đoạn phía sau. Các rủi ro được sinh ra càng sâu trong quá trình phát triển sẽ dẫn đến thiệt hại càng lớn. Ngoài ra, nhóm đã có cơ hội làm quen với việc mô hình hóa yêu cầu qua các loại sơ đồ khác nhau. Bên cạnh đó, nhóm cũng cân nhắc sử dụng Jira cho các dự án sau nhằm quản lý tiến độ vì rõ ràng việc không kịp tiến độ là nhược điểm lớn nhất của dự án lần này. Tóm lại, đây đều là những bài học quý giá có thể áp dụng trong không chỉ các dự án sau này mà còn là môi trường làm việc trong tương lai.
