1. Go to the (C:xampp\php) and open the PHP configuration setting file then find the [mail function] by scrolling down or simply press ctrl+f to search it directly then find the following lines and pass these values. Remember, there may be a semicolon ; at the starting of each line, simply remove the semicolon from each line which is given below.

[mail function]
For Win32 only.
http://php.net/smtp
SMTP=smtp.gmail.com
http://php.net/smtp-port
smtp_port=587
sendmail_from = your_email_address_here
sendmail_path = "\"C:\xampp\sendmail\sendmail.exe\" -t"


2. Now, go the (C:\xampp\sendmail) and open the sendmail configuration setting file then find sendmail by scrolling down or press ctrl+f to search it directly then find the following lines and pass these values. Remember, there may be a semicolon ; at the starting of each line, simply remove the semicolon from each line which is given below.

smtp_server=smtp.gmail.com
smtp_port=587
error_logfile=error.log
debug_logfile=debug.log
auth_username=your_email_address_here
auth_password=your_password_here
force_sender=your_email_address_here (it's optional)
