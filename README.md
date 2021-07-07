Instal PPTPD.

# apt-get install PPTPD Enter



Kemudian kami mengatur IP untuk klien & remote

# /etc/pptpd.conf Enter.

Tempel ini

LocaliP 192.168.100.178.

RemoteP 192.168.100.179-200.



Lalu kita mengedit DNS

# Nano / etc / PPP / PPTPD-Options Enter



Kemudian mengatur IPv4.

# nano sysctl.conf.Enter

Hapus tanda pagar pada net.ipv4.ip_forward = 1

Tempel ini

MS-DNS 8.8.8.8

MS-DNS 8.8.4.4



Lalu kami membuat nama pengguna & kata sandi

# Nano / etc / ppp / chap-recrets Enter

Paste kan ini

Tukangkuli     PPTPD     Tukangkuli     *





Lalu kita restart

# /etc/init.d/pptpd restart. Enter



see here for full tutorial https://tukangkuli707.blogspot.com/2021/07/pptpd-debian.html
