# 魔方财务系统全解密版

本源码是魔方财务系统3.5.8版本全解密版，未进行任何改动。

本源码仅供个人学习研究和交流使用，切勿用于商业用途。

Nginx 伪静态

location / {
 if (!-e $request_filename) {
 rewrite ^(.*)$ /index.php?s=$1 last;
 break;
 }
}