# папка mainserver    
в конфиг Nginx на основном сервере добавить строчку  include /etc/nginx/cloudflare.conf;    
в папку /etc/nginx/ скопировать файлик cloudflare.conf, где прописать локальную подсеть/подсети "маленьких" vds с haproxy. Нужно для отображения реального айпи трафика в логах.
# папка balancer    
готовый конфиг haproxy, адаптирован под cloudflare
HA-Proxy version 1.8.8-1ubuntu0.1 2018/05/29
