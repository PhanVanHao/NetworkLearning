#► Một số câu hỏi ôn tập
##1. Kể tên các thiết bị mạng cơ bản. Chức năng chính.
- 1.1 Repeater
Repeater là thiết bị ở lớp 1 (Physic Layer) trong mô hình OSI. 
Khi chúng ta sử dụng Repeater, tín hiệu vật lý ở đầu vào sẽ được khuếch đại, 
từ đó cung cấp tín hiệu ổn định và mạnh hơn cho đầu ra, để có thể đến được những vị trí xa hơn. 
Nếu bạn muốn đảm bảo tốc độ đường truyền với những khu vực văn phòng làm việc lớn, 
hay sử dụng trong điện tín, truyền thông tin qua sợi quang,... thì bạn nên chọn Repeater.
- 1.2 Hub
Hub sở hữu nhiều cổng từ 4 lên tới 24 cổng, và được coi như là một Repeater nhiều cổng. 
Khi thông tin được truyền tín hiệu vào một cổng của Hub, các cổng khác cũng sẽ nhận được thông tin ngay lập tức.

Hiện nay có 2 loại Hub phổ biến là Active Hub và Smart Hub:

- 1.2.1 Active Hub: loại Hub này thường được dùng phổ biến hơn rất nhiều, cần được cấp nguồn khi hoạt động. 
Active Hub dùng để khuếch đại tín hiện đến và chia ra những cổng còn lại để đảm bảo tốc độ 
tín hiệu cần thiết khi sử dụng.

- 1.2.2 Smart Hub: hay còn gọi là Intelligent Hub cũng có chức năng làm việc tương tự như Active Hub, 
nhưng được tích hợp thêm chip có khả năng tự động dò lỗi trên mạng.

- 1.3 Bridge
Nếu Repeater là lớp thứ nhất trong mô hình OSI thì Bridge là lớp thứ 2 trong mô hình này (Data Link Layer). Công cụ này được dùng để kết nối giữa hai mạng để tạo thành một mạng lớn, chẳng hạn cầu nối giữa hai mạng Ethernet.

Khi có một máy tính này truyền tín hiệu tới một máy khác với hai mạng hoàn toàn khác nhau, 
thì Bridge sẽ sao chép lại gói tin và gửi nó tới mạng đích.


Như vậy, dù các máy tính thuộc mạng khác nhau vẫn có thể 
truyền tín hiệu cho nhau mà không cần biết đến sự xuất hiện của Bridge, do nó hoạt động trong suốt. 
Một Bridge có thể xử lý được nhiều lưu thông trên mạng cũng như địa chỉ IP cùng một lúc. 
Tuy nhiên, Bridge chỉ kết nối những mạng cùng loại và sử dụng cho những mạng tốc độ cao 
sẽ khó hơn nếu chúng nằm cách xa nhau.

- 1.4 Switch
Switch được coi như một Bridge nhiều cổng. Tuy nhiên, Bridge chỉ có 2 cổng làm việc để liên kết 
thì Switch lại có khả năng kết nối được nhiều hơn tùy thuộc vào số cổng có trên Switch. 
Công cụ này có 2 chức năng chính là chuyển các khung dữ liệu từ nguồn đến đích, xây dựng các bảng Switch.
Tốc độ hoạt động của Swtich cao hơn rất nhiều so với Repeater, khả năng hoạt động cũng tích cực hơn do cung cấp nhiều chức năng hơn như tạo mạng LAN ảo (VLAN).

- 1.5 Router
Router được xếp ở lớp thứ 3 của mô hình OSI (Network Layer), có nhiệm vụ kết nối hai hoặc nhiều mạng IP với nhau.

Router kết nối các loại mạng khác nhau,
từ những Ethernet cục bộ tốc độ cao cho đến đường dây điện thoại đường dài có tốc độ chậm. 
Nhưng khả năng làm việc của Router chậm hơn Bridge, 
do cần phải tính toán để tìm ra đường đi cho các gói tín hiệu, 
đặc biệt khi kết nối với các mạng không cùng tốc độ thì lại càng phải cần làm việc nhiều hơn.

- 1.6 Gateway
Gateway kết nối hai mạng có giao thức khác nhau, 
như mạng dùng giao thức IP với mạng sử dụng giao thức IPX, Novell, DECnet, SNA... 
Với những máy tính trong các mạng sử dụng các giao thức khác nhau có thể dễ dàng kết nối được với nhau.

Gateway có khả năng phân biệt các giao thức, ứng dụng khi chuyển thư điện tử từ mạng này sang mạng khác, chuyển đổi một phiên làm việc từ xa.

##2. Mạng máy tính: Định nghĩa, nhu cầu kết nối.
Mạng máy tính là một tập hợp các máy tính được nối với nhau bởi đường truyền 
theo một cấu trúc nào đó và thông qua đó các máy tính trao đổi thông tin qua lại cho nhau. 
Đường truyền là hệ thống các thiết bị truyền dẫn có dây hay không dây 
dùng để chuyển các tín hiệu điện tử từ máy tính này đến máy tính khác.

Nhu cầu kết nối mạng không dây ngày càng tăng phục vụ cho giải trí , truyền thông ,học tập ...

##3. Kể tên các topology mạng. Topo nào đang được sử dụng tại Phòng thực hành Tầng 5 - Học viện Kỹ thuật Mật Mã?
- Bus
- Ring
- Star

tao nghĩ đang dùng mạng hình sao : ) . để hôm sau check lại


##5. Cách mở rộng mạng hình sao, các nguyên tắc cơ bản
- Mở rộng mạng hình sao bằng switch 
- Chỉ cần đủ cổng kết nối là có thể mở rộng 

##6. Kể tên 7 tầng mô hình OSI
7.Application
6.Presentation
5.Session
4.Transport
3.Network
2.Datalink
1.Physical
