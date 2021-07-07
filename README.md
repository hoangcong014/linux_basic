# linux-simple-commands
Note lại những câu lệnh cần dùng trong Linux

# Lệnh kiểm tra file config
sudo sshd -t # kiểm tra file cấu hình etc/ssh/sshd_config

# Clear teminal almost Linux OS
Tổ hợp phím Ctrl và L

# Xoa file, folder
rm "tên file"
rm -r -f "tên folder"

# Tìm kiếm file file/foldir
find / -name "tên cần tìm" # tìm tất file hoặc folder trong thư mục cần tìm, / là thư mục root, ~ là thư mục home của user  
find / -type f -name "tên cần tìm"  # tìm file  
find / -type d -name "tên cần tìm" # tìm folder  
find / -iname "tên cần tìm" # tìm folder hoặc file phân biệt hoa thường  

# Phân quyền người dùng
chmod a-w file (removes all writing permissions)  
chmod o+x file (sets execute permissions for other (public permissions))  
chmod u=rx file        (Give the owner rx permissions, not w)  
chmod go-rwx file      (Deny rwx permission for group, others)  
chmod g+w file         (Give write permission to the group)  
chmod a+x file1 file2  (Give execute permission to everybody)  
chmod g+rx,o+x file    (OK to combine like this with a comma)  

u = user that owns the file  
g = group that owns the file  
o = other (everyone else)  
a = all (everybody)  

r = read aces to the file  
w = write access  
x = execute (run) access   
