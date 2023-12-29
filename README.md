# Skillfolio
 It combines the words "skills" and "portfolio" to represent a collection of your technical skills showcased in a CV format. It conveys the idea of presenting your abilities and accomplishments in a visually appealing and accessible manner.
# Docker
1. Run docker compose
```shell
docker-compose up
```
# WebServer
1. Nginx
```shell
sudo apt-get update
sudo apt-get install nginx
```
2. Add configuration file
```shell
touch /etc/nginx/conf.d/your-project.conf
```
3. Configure Reverse Proxy
```yaml
server {
    listen 80;
    server_name your-domain.com;

    location /api/ {
        proxy_pass http://localhost:8080; # Point to your Spring Boot backend
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
    }

    location / {
        root /path/to/your/frontend/files; # Specify the path to your Angular frontend
        index index.html;
    }
}
```
4. Test configuration
```shell
sudo nginx -t
```
5. Reload Nginx
```shell
sudo systemctl reload nginx
```
6. ##### DNS Configuration:
If your project is accessible via a domain name, make sure to configure your DNS settings to point to the server where Nginx is installed.

7. ##### Firewall and Security:
Review and configure your server's firewall settings to allow traffic on the Nginx ports (usually 80 and 443 for HTTP and HTTPS). Additionally, consider implementing security measures such as TLS/SSL encryption if your project handles sensitive data.

8. ##### Monitoring and Scaling:
Monitor the performance of your Nginx reverse proxy and consider implementing load balancing and caching if needed for scalability.

1. 20230101
2. 20230104
3. 20230107
4. 20230110
5. 20230401
6. 20230404
7. 20230407
8. 20230704
9. 20230707
10. 20230710
11. 20230804
12. 20230807
13. 20230810
14. 20231104
15. 20231107
16. 20231110
17. 20240104
18. 20240107
19. 20240110
20. 20240401
21. 20240404
22. 20240407
23. 20240704
24. 20240707
25. 20240710
26. 20240804
27. 20240807
28. 20240810
29. 20241104
30. 20241107
31. 20241110
32. 20250104
33. 20250107
34. 20250110
35. 20250401
36. 20250404
37. 20250407
38. 20250704
39. 20250707
40. 20250710
41. 20250804
42. 20250807
43. 20250810
44. 20251104
45. 20251107
46. 20251110
47. 20260104
48. 20260107
49. 20260110
50. 20260401
51. 20260404
52. 20260407
53. 20260704
54. 20260707
55. 20260710
56. 20260804
57. 20260807
58. 20260810
59. 20261104
60. 20261107
61. 20261110
62. 20270104
63. 20270107
64. 20270110
65. 20270401
66. 20270404
67. 20270407
68. 20270704
69. 20270707
70. 20270710
71. 20270804
72. 20270807
73. 20270810
74. 20271104
75. 20271107
76. 20271110
77. 20280104
78. 20280107
79. 20280110
80. 20280401
81. 20280404
82. 20280407
83. 20280704
84. 20280707
85. 20280710
86. 20280804
87. 20280807
88. 20280810
89. 20281104
90. 20281107
91. 20281110
92. 20290104
93. 20290107
94. 20290110
95. 20290401
96. 20290404
97. 20290407
98. 20290704
99. 20290707
100. 20290710