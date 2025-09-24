# Buffer-Overflow MS17-010
## Sandbox
- Virtualbox 
- Windows 7

## Tools
- Wireshark 
- Nmap 
- Metasplots

# pcap analysis
## Scanning
Liên tục có các gói Syn được gửi đến các port khác nhau, điều này cho thấy có ai đó đang scan hệ thống của chúng ta 
![alt text](assets/image.png)

## Attack
Nhận thấy có bất thường ở giao thức SMB, khi kiểm tra cá gói tin, ta thấy một chuỗi dài chứa hàng loạt các ký tự A, điều này cho thấy, hacker đang tấn công bằng cách khai thác lỗi Buffer Overflow 
![alt text](assets/image-1.png)