#intro
follow certification CCNA : Routing & Switching
Học xong nên làm : SI (system Integration)
hoặc làm trong ISP
-Ltr Admin Network

- CCNA-CCNP -- CCIE

Sử dụng GNS3 trên window
Cisco IOU trên Linux (centOS)

[Knowledge] INE--blog.ine.com / Documentsanddownload--careercert.info or http://www.net130.com/
# #1.Mạng căn bản
#Mạng
-Mạng là hệ thống đường truyền kết nối các thiết bị khác nhau
để truyền tin , dữ liệu( các thiết bị đầu cuối kết nối vào internet)
+các thành phần thường thấy : PC,Wireless devices,Headquater of company , Branch of company
+các thiết bị thường thấy : PC, đường truyền,switch,router,hub,repeater,...
#Network Diagram
-PC→Network Card interface → RJ45 →Cable →switch → Router → Internet cloud 
-Các giao thức : SSH,VPN
cách gọi : unindenify là cloud 
Dường zikzak : lease line - kênh thuê riêng đấu 2 con router cách xa nhau hàng ngàn cây số
#Sharing Functions
-Data and application ( file , internet game )
-Source ( Printer , fax ......)
-Network storage
-Backup devices
#Network user applications (ứng dụng cần mạng )
-Email
-Browser
-Instant messenging
-Collaboration ( group work: netmeeting )
-Databases(file servers)
#Impact of user applications on the network ( Các loại ứng dụng và đặc tính mạng) 
##Batch applications
-FTP,TFTP,inventory updates
-no direct human interaction
-Bandwidth important , but not critical ( deley allow)
##Interactive apps
-Inventory inquiries, Database updates ( kiểm kê )
-Human-to-machine interaction
-allow a little delay 
##Real-time apps
-VoIP,video call
-Human-to-Human app
-Non-allowed Delay 
độ chờ : latency
#Characteristics of a Network ( đặc tính kĩ thuật ) 
-Speed (băng thông)
-Cost
-Security (bảo mật)
-Availability (sẵn sàng, luôn luôn thường trực k ? Tính dự phòng?)
-Scalability ( có khả năng mở rộng ra không? )
-Reliability ( độ tin cậy đường truyền , chất lượng mạng , có mất gói tin hay không ? )
-Topylogy ( sơ đồ mạng )
	+Physical :	Bus : all receive the signal , can be upgrado to duel ring
			Ring(vòng) : signal travel around ring / tính chất : single point of failure
			Star : tranmission through a central unit(point)(single point of failure)could be upgrade to Extended star topology
	+Logical  :	
##Kiến trúc đấu nối :	 Full-mesh topology : đắt , tính dự bị cực kì cao 
			 Partial Mess : đấu nối 1 số điểm cần - Trade-off ( thỏa hiệp ) between fault-toleration and cost
#Connect to the internet
-PC→Modem→DSL→Internet
-PC→Modem cable→ Cable → Internet
-PC→CSU/DSU → Serial → Internet ( call by Lease line )
# #2.OSI division of layers ( mô hình phân lớp )
#Understanding Host-to-Host communications
##Host
- Là một thực thể mạng có thể truyền được các ứng dụng (PC,server[telnet , ftp,tftp...])
##
-Older model
+Proprietary and "apps and combine by one vendor"
( độc quyền hãng , chỉ dùng kết nối với hãng và sử dụng software của hãng)
-New model : Standards-base model
+Multivendor software
+Phương pháp phân lớp: OSI ( Open system interconnection )mỗi lớp có tính năng riêng hỗ trợ cho các lớp khác
7.Application : Network processes to applications
-Provides network service : cung cấp dịch vụ mạng như mail, transfer ,terminal emulaltion(truy nhập từ xa )
-User authentication :Cơ chế xác thực người dùng 
6.Presentation : -Data presentation : Thông ngôn giữa các ứng dụng
+Format data : Định dạng
+Structures data :Cấu trúc ứng dụng
+Negotiation data transfer and syntax for apps layer : thương lượng phương pháp truyền
+Provides Encryption : cung cấp cơ chế mã hóa
5.Session: Interhost communications : tổ chức phiên kết nối cho các ứng dụng 
Establishes,manages and terminal session between apps

4.Transport : -End-to-end connections : quản lý các kết nối đầu cuối
+ Handle transportation issues : xử lí các vấn đề truyền dẫn
+ Ensure data transport reliability : đảm bảo tin cậy trong truyền dữ liệu
+ Established,maintains,and terminal virtual circuits : thiết lập, duy trì và giải phóng kết nối mạch ảo 
+ Provides reliability through fault detection and recovery infomation flow control : cung cấp tìm lỗi và sửa lỗi 
3.Network   : Chứa các giao thức định tuyến làm việc dựa trên IP(địa chỉ logic)
-Data delivery : +Route data packets: định tuyến cho các gói dữ liệu
		 +Select best path to deliver data : chọn đường đi tốt cho dữ liệu


2.Datalink  : Làm việc dựa trên MAC
-Access to media : điều khiển việc truy nhập vào đường truyền vật lý và giao tiếp với lớp network,
quy định về việc đóng khung dữ liệu, cấu trúc dữ liệu, điều tiết cách dữ liệu từ các lớp trên truy nhập vào lớp vật lý
gắn frame, cung cấp cơ chế dò lỗi 
1.Physical  : Binary tranmission truyền dòng bit thô qua một đường truyền vật lý . 
chỉ quan tâm đến vật lý ( cáp mạng,đầu dây,khoảng cách,voltage,công nghệ truyền,tốc độ vật lý ...)
 

###Ưu điểm
-Reduces complexity (giảm thiểu độ phức tạp do công việc được chia ra )
-Standardizes interfaces ( nền tảng đặc tính kĩ thuật, chuẩn hóa giao diện, tương thích công nghệ )
-Facilitates modular engineering ( chuyên môn hóa, thúc đẩy sự phát triển công nghệ mạng )
-Ensures interoperable techology (=)
-Accelerate Evolution		 (=)
-Simplifies teaching and learning ( dễ dàng cho việc dạy và học )

Mô Hình OSI (Ảnh dưới )

#Data Encapsulation 
-Từ Sender :Dữ liệu đi từ lớp 7 xuống lớp 1 , mỗi lớp đóng thêm 1 số giao thức để chuyển đi 
Header : thông tin quản lý gói tin 
Lớp 2 đóng thêm 1 cái FCS : để kiểm tra lỗi gói tin
Tại lớp 1 dữ liệu được thể hiện dưới dạng bit
-Từ Receiver:Dữ liệu đi từ lớp 1 lên lớp 7 , dần giải phóng các header và nhận được gói thông tin cần nhận

##Peer-to-Peer communication : truyền thông ngang hàng 
Tên gọi gói tin :
- Physical : Bits
- Datalink : Frame
- Network : Packgets
- Transport : Segments


#TCP/IP Stack : mô hình TCP/IP
4.Application [gom 3 nhóm đầu OSI]
3.Transport	
2.Internet	[Network OSI]
1.Network Access [Physical+Datalink]


#Note : ngoài thực tế thì sử dụng mô hình TCP/IP nhưng khi tham chiếu lại dùng OSI 
2 cái là 1 
