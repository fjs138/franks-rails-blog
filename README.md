# Frank's Rails' Blog
A blog developed in Ruby, powered by Rails, a server-side web application framework.<br>
It utilizes <code>http_basic_authenticate_with</code> for authentication to prevent unauthorized users from modifying content.
# Technology Stack:


| Technology    	| Use           	  | Description     										  |
| :------------------|:-------------------| :----------------										  |
| Ruby on Rails 			| Backend     | Server-side, web application (MVC) framework				  |
| SQLite3			| Database			  |	Not a client–server database engine; it is embedded into the end program.            |
| http_basic_authenticate_with			| Authentication			  |	HTTP Basic authentication.            |




# Project Specifications

Create articles

List articles

Display articles

Delete articles

Add comments about a given article

View comments for a given article


# Anatomy of Project


| File/Folder    	| Purpose           	  |
| :------------------|:-------------------|
| app/	 			| Contains the controllers, models, views, helpers, mailers, channels, jobs, and assets.     |
| bin/		 			| Contains the rails script that starts the app and can contain other scripts used to setup, update, deploy, or run your application.    |
| config/		 			| Configures the application's routes, database, and more.    |
| config.ru		 			| 	Rack configuration for Rack based servers used to start the application.     |
| db/			 			| 	Contains the current database schema, as well as the database migrations.    |
| Gemfile, Gemfile.lock		 			| 	These files allow you to specify what gem dependencies are needed for your Rails application. These files are used by the Bundler gem.     |
| lib/			 			| 	Extended modules for the application.    |
| log/			 			| 	Application log files.     |
| package.json			 			| 	This file specifies what npm dependencies are needed for  Rails application. This file is used by Yarn.    |
| public/			 			| 	Viewable by "the world". Contains static files and compiled assets.     |
| Rakefile			 			| 	Locates and loads tasks that can be run from the command line. The task definitions are defined throughout the components of Rails. Rather than changing Rakefile, you should add your own tasks by adding files to the lib/tasks directory of your application.  |
|README.md			| 	Extended modules for the application.                 |
|storage/		 	| 	Extended modules for the application.                 |
| test/			 	| 	Unit tests, fixtures, and other test apparatus.       |
| tmp/			 	| 	Temporary files (like cache and pid files).           |
| vendor/		 	| 	Third-party code; vendored gems.                      |
| .gitignore		| 	Tells git which files (or patterns) it should ignore. |
| .ruby-version	| 	Contains the default Ruby version.                    |

## The actions that users can perform are mapped to routes as follows:
| Prefix       |Method| URI Pattern             	  | Controller#Action|
| :------------------ |:-------------------         | :----------------										  |:----------------										  |
|welcome_index |GET   |    /welcome/index(.:format)  |   welcome#index|
|     articles |GET   |   /articles(.:format)    |      articles#index|
|              |POST  |  /articles(.:format)    |      articles#create|
|  new_article |GET   | /articles/new(.:format)   |   articles#new|
| edit_article |GET   |/articles/:id/edit(.:format) |articles#edit|
|      article |GET   | /articles/:id(.:format)   |   articles#show|
|              |PATCH | /articles/:id(.:format)     | articles#update|
|              |PUT   | /articles/:id(.:format)     | articles#update|
|              |DELETE| /articles/:id(.:format)   |   articles#destroy|
|         root |GET   | /  |                          welcome#index|


# Instructions
Start the application by running `npm start` from within the `redditclone` folder.
Ttart the server by invoking bin/rails server followed by using a web browser to connect to http://localhost:3000/articles
<br><br>
Note:
Credentials for logging in are: "name": "frank", "password": "secret",
<br>
<br><br>


# License
MIT License

Copyright (c) 2015 Frank Santaguida

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
