# SimpleNginxContainer

This is just a simple nginx container serving static website. tic tac toe game. Moving static files to docker container by bind mount the static folder to the nginx static serving folder.
Command 1(to start and see the nginx container): docker --name mynginx -d -p 3000:80 nginx
Command 2: docker --name mynginx -d -p 3000:80 -v "absolute_path_to_static_folder:/usr/share/nginx/html" nginx
