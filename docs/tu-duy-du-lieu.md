Nhiều người thường bảo làm DA ko phải chỉ biết dùng tool mà cần có tư duy logic, tư duy phân tích insight.... bla bla. Vậy thì cái tư duy ấy là gì? Mình xin chia sẻ góc nhìn từ kn làm việc.

Sai lầm có lẽ các bạn DA sẽ hay gặp phải đó là không hiểu yêu cầu của doanh nghiệp hoặc của khách, sai từ bước ban đầu dẫn đến kết quả báo cáo của mình không đưa ra những thông tin có giá trị với họ. Do vậy các bạn khi làm nghề cần hiểu và xác định được yêu cầu và mục tiêu phân tích dữ liệu của doanh nghiệp hoặc của khách hàng. Ko phải tự nhiên mà những bạn background kinh tế có lợi thế hơn trong nghề DA, và các công ty ưu tiên tuyển người có domain trong lĩnh vực của cty.

Vậy ngay ở bước xác định yêu cầu phân tích, làm thế nào để đảm bảo có hướng giải quyết bài toán đúng? Mình xin chia sẻ kinh nghiệm làm mà mình đã học hỏi đc và hay áp dụng trong việc phân tích dữ liệu

**(1)** Khi mới phân tích tại 1 tổ chức doanh nghiệp, cần nắm được mô hình kinh doanh và vẽ quy trình nghiệp vụ Khi mới vào phân tích dữ liệu ở 1 công ty, sẽ có bạn bị bị bối rối, không hiểu các số liệu của công ty, không biết lấy dữ liệu từ đâu. Do đó, trước hết các bạn cần hiểu được mô hình kinh doanh của công ty và vẽ ra quy trình nghiệp vụ của công ty đó.

Ví dụ như trong trung tâm Tiếng Anh, mô hình hoạt động của họ là kết nối với giáo viên, mở các lớp dạy tiếng Anh (sản phẩm) và tuyển sinh học viên (khách hàng). Hiện đang có 2 lớp IELTS for newbie, giờ sếp muốn mở thêm 3 lớp đấy, muốn bạn phân tích để tính ra được KPI mà marekting và sales cần đạt được để tuyển sinh đủ lớp.

![➡️](https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/27a1.png "Right arrow    :arrow_right:") Vậy thì bạn cần nắm được cả quy trình tuyển sinh (bán hàng) của họ, thì mới biết hướng phân tích từ đâu (lấy chỉ số từ sales tính ra KPI cho marketing hay ngược lại?) và hiểu tất chỉ số mà họ quy ước (ví dụ: L1 là kh mới đăng ký, L2 là đã sale đã gọi, L3 là khách hàng có quan tâm, L4 là khách muốn học, L5 là khách đã chốt hợp đồng), biết liên hệ với bộ phận nào để khai thác thông tin mình cần.

**(2) Tư duy phân tích dữ liệu đa chiều

Phân tích đa chiều là gì?** Cùng 1 chủ điểm phân tích, chúng ta sẽ xem xét dưới nhiều góc nhìn khác nhau (doanh số chi tiết theo từng sản phẩm là bao nhiêu, theo từng khu vực, từng quý là bao nhiêu,..., hoặc chi tiết hơn nữa vd như chi tiết doanh thu theo doàng sản phẩm A trong quý 2 là bao nhiều). Khi chúng ta có thể trả lời những câu hỏi đấy 1 cách nhanh chóng theo thời gian thực bằng dashboard hoặc các phân tích BI, thì đấy gọi là phân tích đa chiều. Các bước phân tích đầu bài với phương pháp phân tích đa chiều

![✔️](https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/2714.png "Check mark    :heavy_check_mark:")Bước 1: Xác định Dim - Fact

Trước hết, Fact là các chủ điểm phân tích dữ liệu từ yêu cầu, ví dụ yêu cầu phân tích doanh số và sản lượng bán ra trong năm nay, thì doanh số và sản lượng chính là Fact.

Dimension là các khía cạnh phân tích. Ví dụ phân tích doanh số, chúng ta có thể xem xét theo chiều thời gian (theo quý, theo tháng), theo khu vực (các chi nhánh), theo danh mục loại sản phẩm, theo nhân viên bán hàng,...

![✔️](https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/2714.png "Check mark    :heavy_check_mark:")Bước 2: Cần liệt kê các giá trị trong Dimension.

Ví dụ theo dimension Thời gian thì ta có các giá trị trong đó là: Tháng 1, Tháng 2, Tháng 3,... (Hoặc quý 1, quý 2,...)

Theo dimension sản phẩm thì ta có giá trị trong đó là: Sản phẩm A, Sản phẩm B, Sản phẩm C,...

Theo dimension khu vực thì trong đó ta có: Hà Nội, Hồ Chí Minh, Đà Nẵng,...

![9405904f-1082-46da-b856-94aa2c8b5eee.png](https://voz.vn/proxy.php?image=https%3A%2F%2Fimages.viblo.asia%2F9405904f-1082-46da-b856-94aa2c8b5eee.png&hash=7f9054dacd52dcf3dbc6ebc4778e87fa "9405904f-1082-46da-b856-94aa2c8b5eee.png")

![✔️](https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/2714.png "Check mark    :heavy_check_mark:")Bước 3: vẽ mô hình dữ liệu cho hệ thống phân tích dữ liệu

Bên tay phải có Fact (chủ điểm phân tích), và bên tay trái là Dim (chiều dữ liệu). Trong mô hình này, chúng ta hệ thống lại các chiều dữ liệu và các cấp nhỏ hơn của mỗi chiều. Cùng với đó là sự liên hệ với các chủ điểm phân tích trong hệ thống dữ liệu.

![⚪](https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/26aa.png "White circle    :white_circle:") Ví dụ khi phân tích dòng sản phẩm A và ở thị trường quốc gia VN, thì chúng ta có thể phân tích về doanh số, lượng tồn kho,...

![⚪](https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/26aa.png "White circle    :white_circle:") Ví dụ phân tích về giá, chúng ta không phân tích theo cửa hàng mà phân tích theo dòng sản phẩm và theo thời gian (năm, quý). Phân tích về sức mua (purchase amount) thì sẽ phân tích theo khu vực, theo dòng sản phẩm và theo thời gian, chứ không phải theo khách hàng

![48045ada-fdfe-42fc-b045-5d893a5bfc1e.png](https://voz.vn/proxy.php?image=https%3A%2F%2Fimages.viblo.asia%2F48045ada-fdfe-42fc-b045-5d893a5bfc1e.png&hash=f5054e70eca6f16aab5726bb848369d8 "48045ada-fdfe-42fc-b045-5d893a5bfc1e.png")

![❓](https://cdn.jsdelivr.net/gh/twitter/twemoji@14.0.2/assets/72x72/2753.png "Question mark    :question:") Tại sao cần vẽ Data Model dạng này? Mô hình này giúp dễ dàng xác định các nhu cầu phân tích, nhu cầu làm báo cáo và xây dựng chủ điểm phân tích dễ dàng hơn.

Bên cạnh đó nó giúp hình dung các chiều dữ liệu rõ ràng hơn.

Nếu bạn chỉ cần làm 1 báo cáo nhanh bằng Excel thì việc xây dựng Data Model kiểu này giúp bạn nắm được tổng thể các chiều dữ liệu và sự liên kết trong các dữ liệu. Việc kéo thả vào pivot table, kéo thả các bar chart trong BI trở nên dễ dàng hơn. Giúp quá trình xây dựng dash tổng thể và khoa học hơn rất nhiều

Nếu bạn cần xây dựng dashboard phức tạp trên Power BI, thì mô hình này giống như 1 bản mô phỏng, giúp bạn xây dựng Data Model đầy đủ và chuẩn xác hơn