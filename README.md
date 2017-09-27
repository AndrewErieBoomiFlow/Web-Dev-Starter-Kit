
# PHP / Apache Docker Start Template

This is a simple way to get php running locally without much setup.

1. Install docker : https://www.docker.com/

2. Open your console / terminal and navigate to where you've downloaded this project.

2. Build the project (change mysite to whatever you want the image to be called)
```
docker build -t mysite .
```

3. Run the project (With Mount) 
```
docker run -p 8080:80 -d -v /users/you/projectFolder/www:/var/www/site mysite
```

4. View in browser
```
http://localhost:8080/
```