<h3>About</h3>
This repository can be used to install <a href="https://github.com/zus1/todo_list">Todo list</a> project directly for github, using docker compose.
This way is also preferred way of running Todo list project.
<h3>Install and Run</h3>
Set up can be done in three steps. <br><br>

First one is to clone this repository
<pre><code>git clone https://github.com/zus1/todo_list-composer.git local_directory</code></pre>
Second step is run docker containers
<pre><code>docker-compose up</code></pre>
And last is, bash into web container and run migrations
<pre><code>docker container exec -it todo_web bash</code></pre>
<pre><code>php bin/console doctrine:migrations:migrate</code></pre>
And now you should be ready to fly. Go to localhost:8081 and site should be up :) 
<br><br>
For more info about Todo list project, you can check its own repository 
<a href="https://github.com/zus1/todo_list">here</a>
