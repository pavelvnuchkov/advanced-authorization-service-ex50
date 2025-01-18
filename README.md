  location /signin {
	alias html;
	index authorization.html;
	
       }

 location / {
            root   html;
           index index.html index.htm;
           proxy_pass http://localhost:8080;
        }
