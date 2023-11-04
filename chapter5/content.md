- Rem, em, px
rem, em, và px là ba đơn vị đo lường trong CSS được sử dụng để xác định kích thước, khoảng cách và các giá trị liên quan đến kích thước. Dưới đây là sự khác nhau giữa chúng:

px (Pixel): px là đơn vị đo lường tuyệt đối và không phụ thuộc vào bất kỳ yếu tố nào khác ngoài nó. Một giá trị 10px sẽ luôn có kích thước 10 pixel trên màn hình, không quan tâm đến các yếu tố bên ngoài.

em: em là một đơn vị tương đối dựa trên kích thước của phần tử cha gần nhất của phần tử đang được áp dụng. Nếu bạn đặt một giá trị là 1em cho một phần tử con, nó sẽ có kích thước bằng với kích thước của phần tử cha. Nếu bạn đặt giá trị là 2em, nó sẽ gấp đôi kích thước của phần tử cha.

rem (Root em): rem là một đơn vị tương đối giống em, nhưng nó dựa trên kích thước của phần tử gốc (root) của trang web (thường là phần tử <html>). rem giúp bạn kiểm soát kích thước phần tử dựa trên cơ sở toàn bộ trang web mà không bị ảnh hưởng bởi kích thước của các phần tử cha.

Ví dụ về sự khác nhau giữa em và rem:

Nếu bạn có một phần tử cha với kích thước là 20px và bạn đặt một phần tử con với kích thước là 1em, phần tử con sẽ có kích thước là 20px. Tuy nhiên, nếu bạn đặt kích thước của phần tử con là 1rem, nó sẽ có kích thước dựa trên kích thước gốc của trang web, không phụ thuộc vào phần tử cha.

Lựa chọn giữa em, rem, và px phụ thuộc vào ngữ cảnh thiết kế và yêu cầu cụ thể của trang web hoặc ứng dụng của bạn.

- VW vs 100%
VW (Viewport Width): "vw" đo kích thước dựa trên chiều rộng của viewport (khung nhìn) của trình duyệt. 1vw tương đương với 1% của chiều rộng của viewport. Ví dụ, nếu bạn đặt một phần tử có chiều rộng là 50vw, nó sẽ chiếm 50% chiều rộng của viewport. "vw" là một cách để điều chỉnh kích thước dựa trên kích thước của màn hình.

100%: "100%" đo kích thước dựa trên phần tử cha của phần tử đó. Khi bạn đặt một phần tử con có chiều rộng là 100%, nó sẽ chiếm toàn bộ chiều rộng của phần tử cha. Điều này làm cho phần tử con bằng chiều rộng của phần tử cha mà nó được đặt bên trong.

Ví dụ, nếu bạn có một phần tử con được đặt trong một phần tử cha và bạn muốn phần tử con chiếm toàn bộ chiều rộng của phần tử cha, bạn có thể sử dụng "width: 100%;" cho phần tử con. Trong khi đó, "vw" sẽ cho phép bạn điều chỉnh kích thước dựa trên kích thước của viewport và không phụ thuộc vào phần tử cha.

- box-sizing là một thuộc tính CSS quan trọng được sử dụng để quyết định cách các phần tử xác định kích thước của nó và cách tính toán kích thước đó. Thuộc tính box-sizing có hai giá trị quan trọng:

- content-box (Giá trị mặc định): Khi bạn sử dụng box-sizing: content-box;, phần tử tính toán kích thước của nó dựa trên nội dung bên trong và thêm các giá trị của padding và border vào nó. Điều này có nghĩa là nếu bạn đặt một kích thước cố định cho một phần tử, thì padding và border sẽ làm cho phần tử trở nên lớn hơn so với kích thước cố định đó.

- border-box: Khi bạn sử dụng box-sizing: border-box;, phần tử tính toán kích thước của nó bằng cách tính toán từ đỉnh của border đến đỉnh của border. Nó không tính thêm padding hoặc border vào kích thước của phần tử. Điều này giúp giữ cho kích thước của phần tử cố định, và bất kỳ padding hoặc border sẽ thay đổi kích thước nội dung bên trong, thay vì làm thay đổi kích thước tổng thể của phần tử.

Việc sử dụng box-sizing thường hữu ích trong việc quản lý layout và thiết kế trang web. Nó cho phép bạn kiểm soát cách phần tử phản ứng với padding và border, giúp đảm bảo tính đồng nhất và dễ quản lý trong việc thiết kế trang web.
