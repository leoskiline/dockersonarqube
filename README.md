# dockersonarqube
Docker - SonarQube - Nginx - Certbot - PostgreSQL

Step 1:
Remove server listening on port 443 in /nginx/app.conf.

Step 2:
Change staging to 1 on init-letsencrypt.sh to verify successful of getting certificate before get definitely.

Step 3:
Run init-letencrypt.sh and verify operation successful.

Step 4:
If operation successful, Change staging to 0 on init-letsencrypt.sh, this will get certificate definitely for your domain.

Step 5:
After obtain certificate with success, Go to /nginx/app.conf and add server listening on port 443.

Step 6:
Well done, run docker-compose up and use you application secure.
