# OSU Lazer

## Phân tích dự án trò chơi âm nhạc trực tuyến osu!lazer

### 1. Bối cảnh

- **osu!** (hay **osu!stable**) là tựa game âm nhạc được ra mắt trên nền tảng PC vào năm 2007 bởi Dean "peppy" Herbert dựa trên trò chơi cùng tên (Osu! Tatakae! Ouendan!) được phát hành trên Nintendo DS vào năm 2005. Dự án gây được tiếng vang lớn nhờ gameplay dễ gây nghiện nhưng cũng đầy thử thách, nhiều chế độ chơi khác nhau cũng như một cộng đồng lớn mạnh. Theo thống kê trên trang chủ của tựa game ([https://osu.ppy.sh](https://osu.ppy.sh)) vào 16/10/2025, ở Việt Nam có khoảng 57,022 người chơi hoạt động thường xuyên với tựa game này.
- Tuy nhiên, do được thiết kế và lập trình trên nền tảng công nghệ cũ, tuy vẫn đang hoạt động cho đến thời điểm hiện tại nhưng trò chơi vẫn mắc phải một số điểm bất cập như việc tình trạng giật lag xảy ra thường xuyên, mất kết nối đến máy chủ cũng như chế độ nhiều người chơi hoạt động thiếu ổn định. Song song với đó, tựa game cũng bị giới hạn về công nghệ và khả năng mở rộng. Để khắc phục những điểm yếu kể trên cũng như giúp tựa game phù hợp hơn với thời đại, vào năm 2017, peppy đã ra mắt dự án **osu!lazer** với nhiều hứa hẹn đến từ chính nhà phát triển. Tuy nhiên sau 8 năm xây dựng, đến hiện tại tựa game vẫn chưa thể đưa được cho cộng đồng một phiên bản trò chơi tương xứng với kì vọng.
- Dự án được phát hành dưới dạng **mã nguồn mở trên GitHub**, được phát triển liên tục dưới sự đóng góp của cộng đồng.

### 2. Phạm vi

- Mục tiêu xuyên suốt của osu!lazer là **viết lại toàn bộ kiến trúc của tựa game cũ** bằng những công nghệ hiện đại hơn (.NET 6, cross-platform, UI framework riêng,...) nhằm mục đích tối ưu hóa hiệu năng cũng như khả năng mở rộng và đa nền tảng (Windows, Linux, MacOS, Android và IOS). Đồng thời, trò chơi cũng **giữ gìn gameplay cốt lõi** đi kèm **với nhiều tính năng mới** như chế độ chơi trực tuyến được mở rộng, thêm các mod mới để thay đổi gameplay, khả năng tự tạo các chế độ chơi mới thông qua ruleset API,...
- Tuy phạm vi lớn là vậy, dự án vẫn có **lộ trình rõ ràng và công khai** trên GitHub, được chia thành các **cột mốc (milestone)** như framework, engine, UI, gameplay và hệ thống trực tuyến, thể hiện khả năng quản lý phạm vi hiệu quả.

### 3. Tiến độ (Schedule)

- Dự án được khởi động từ **năm 2017**, và vẫn đang trong quá trình phát triển sau **8 năm** ròng rã. Tuy vậy, người chơi vẫn được tiếp cận với tựa game thông qua các bản cập nhật nhỏ hàng tuần được phát hành thông qua GitHub Actions.
- Dự án được phát triển mã nguồn mở, mọi tính năng đều được thiết kế, thử nghiệm và phải hồi **công khai** trên GitHub, khiến tiến độ chậm hơn nhưng được **chất lượng và minh bạch.**
- Phần lớn thời gian phát triển cũng được phân bổ cho việc chuẩn hóa gameplay, chuyển đổi dữ liệu cũ, và tối ưu hóa khả năng hoạt động đa nền tảng (Windows, macOS, Linux, Android, iOS).
- Bên cạnh đó, đội ngũ phát triển osu!lazer cũng có phần khiêm tốn về mặt số lượng nhân sự, phần nào đó cũng ảnh hưởng đến quá trình hoàn thiện trò chơi.

### 4. Chi phí và nguồn lực

- osu!lazer -- cũng như phiên bản trước đó -- là dự án **mã nguồn mở và phi lợi nhuận**. Tất cả những chi phí liên quan đến nhân sự, duy trì trò chơi đều đến từ đóng góp tự nguyện thông qua osu! supporter (một hình thức đăng kí tính năng có trả phí) và các khoản ủng hộ khác nhau. Những người chơi có trình độ tin học cao hơn có thể đóng góp vào dự án thông qua việc trở thành các Developer Volunteer -- trực tiếp tham gia vào quá trình phát triển trò chơi.
- Nhờ vào đó, dự án **không phải chịu áp lực lớn về tài chính** như các dự án game thương mại khác -- hay nói cách khác, dự án được tự do để toàn lực dốc sức vào chính chất lượng của trò chơi thay vì phải chịu sự áp lực hay giám sát từ các nhà đầu tư.
- Tuy vậy, việc phụ thuộc lớn vào tinh thần đóng góp tự nguyện của trò chơi cũng mang lại một số **hạn chế** cho chính bản thân dự án như ảnh hưởng đến tiến độ phát triển, gây phân tán nguồn lực kĩ thuật hay rủi ro về việc duy trì ổn định lâu dài.
- Đến hiện tại, mô hình vẫn chứng minh được tính bền vững và sức ảnh hưởng của osu!, trở thành một ví dụ điển hình về **cách một dự án cộng đồng có thể phát triển quy mô toàn cầu mà không cần mô hình thương mại truyền thống**.

### 5. Chất lượng

- Dự án làm lại của tựa game cũ có **một số điểm cải thiện đáng kể**: Giao diện trò chơi đẹp, thân thiện và dễ nhìn hơn so với bản cũ; các tính năng chơi được mở rộng và khả năng tùy biến cao; hỗ trợ đa nền tảng.
- Tuy vậy, phần lớn người chơi **vẫn chọn ở lại với phiên bản stable của trò chơi**, cho rằng dự án mới vẫn đang quá thiếu hoàn thiện. Điều này có thể thấy ở rất nhiều điểm bất cập của lazer: Thiếu đi một số tính năng quan trọng, đặc biệt là trình biên tập map chơi; yêu cầu cấu hình cao hơn so với tựa game gốc; các vấn đề về tương thích với các map chơi/skin ở phiên bản cũ. Đặc biệt, dù được tối ưu về mặt công nghệ, tựa game mới vẫn thiếu đi độ ổn định; các yếu tố về giật lag vẫn hay xảy ra, một số tính năng cũ ở gameplay hoạt động thiếu nhất quán và vấn đề nghiêm trọng nhất là **độ trễ đầu vào (input latency)** -- yếu tố ảnh hưởng trực tiếp đến độ chính xác trong một tựa game dựa vào nhịp điệu âm nhạc.
- Với các yếu tố trên, có thể nói dự án lazer vẫn chưa thể thay thế hoàn toàn phiên bản cũ, người chơi -- đặc biệt là các streamer chuyên nghiệp và người chơi thi đấu -- vẫn trung thành hơn với phiên bản cũ, vốn mang lại cảm giác chơi ổn định, chính xác và đáng tin cậy hơn.

### 6. Rủi ro

- Mô hình phát triển mở và phi lợi nhuận khiến osu!lazer **phụ thuộc mạnh vào tinh thần đóng góp tự nguyện của cộng đồng**. Nếu sự quan tâm giảm sút, tiến độ có thể bị chậm lại hoặc gián đoạn. Bên cạnh đó, sự phân tán về nhân lực và trình độ kỹ thuật giữa các cộng tác viên cũng dẫn đến khó khăn trong việc duy trì chất lượng mã nguồn thống nhất, dễ phát sinh lỗi hoặc xung đột phần mềm.
- Do dự án phát triển song song với phiên bản stable, nguy cơ **chia rẽ cộng đồng người chơi** là hiện hữu: một bộ phận ủng hộ lazer, trong khi phần lớn vẫn trung thành với phiên bản cũ vì tính ổn định. Điều này xuất phát từ việc lazer vẫn đang trong giai đoạn hoàn thiện làm cho rủi ro về trải nghiệm người dùng khá cao, điều này có thể ảnh hưởng tiêu cực đến uy tín của trò chơi nếu không được khắc phục triệt để.
- Về lâu dài, nếu không có chiến lược chuyển đổi người dùng hoặc nguồn lực ổn định hơn, dự án có thể **rơi vào tình trạng "phát triển kéo dài"** mà không đạt đến giai đoạn phát hành chính thức.

### 7. Bài học rút ra

- Dự án osu!lazer vốn có rất nhiều tiềm năng để thay thế người đàn anh của mình để trở thành phiên bản kế nhiệm xứng đáng của trò chơi nổi tiếng, tuy vậy tựa game mới vẫn để lại nhiều điều tiếc nuối sau 8 năm dài đã và đang phát triển. Từ đó, ta có thể rút ra được nhiều bài học sâu sắc về quản lý dự án và phát triển phần mềm quy mô lớn.
- Trước hết, việc **xác định phạm vi và lộ trình hợp lý** là yếu tố then chốt. Dự án lazer đặt mục tiêu quá rộng -- viết lại toàn bộ trò chơi, chuyển sang công nghệ mới, hỗ trợ đa nền tảng và mở rộng hệ thống gameplay -- dẫn đến tiến độ kéo dài nhiều năm. Điều này cho thấy tầm quan trọng của việc **phân chia mục tiêu thành từng giai đoạn rõ ràng**, có thể kiểm soát và đánh giá được.
- Bên cạnh đó, **công nghệ hiện đại không đảm bảo ngay lập tức mang lại trải nghiệm tốt hơn**. Dù osu!lazer áp dụng .NET 6 và kiến trúc tiên tiến, phần lớn người chơi vẫn trung thành với phiên bản stable vì sự ổn định, quen thuộc và độ chính xác cao. Từ đó có thể thấy, trong phát triển sản phẩm, **sự đổi mới kỹ thuật cần đi đôi với việc thấu hiểu nhu cầu và thói quen của người dùng**.
- Dự án cũng minh chứng rằng **mô hình mã nguồn mở** tuy mang lại tính tự do và minh bạch, nhưng đòi hỏi **năng lực điều phối và tổ chức cộng đồng hiệu quả**. Khi nguồn lực đến từ đóng góp tự nguyện, việc duy trì tiến độ, kiểm thử và chất lượng phần mềm trở nên khó khăn hơn đáng kể.
- Cuối cùng, **osu!lazer nhấn mạnh tầm quan trọng của tính ổn định và hiệu năng** trong các trò chơi nhịp điệu. Chỉ cần sai lệch nhỏ về độ trễ đầu vào cũng có thể ảnh hưởng lớn đến trải nghiệm người chơi. Một sản phẩm bền vững không chỉ dựa vào công nghệ mới, mà còn vào **sự kiên trì, lắng nghe phản hồi và tầm nhìn dài hạn của đội ngũ phát triển**.
