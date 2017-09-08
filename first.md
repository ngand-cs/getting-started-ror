First thing, a few concept:

- rvm and rbenv are managers. They allow you to mannage multiple installations
  of Ruby.
- Gem look same as npm in Nodejs
- `bundle command` same as command `npm install`
- Gemfile same as package.json in Nodejs.

#### Install Ruby

- In Debian or Ubuntu: `sudo apt-get install ruby-full`
- In Centos, Fedora: `sudo yum install ruby`
- Build from source:
Download the source code from: https://www.ruby-lang.org/en/downloads/
```
$ ./configure
$ make
$ sudo make install
```
By default, this will install Ruby into /usr/local. To change, pass the
--prefix=DIR option to the ./configure script.


#### Install Rail

With specific version number `gem install rails -v 5.1.2`

#### First Application

`rails new hello_app`

List of directory:

|   	|   	|
|---	|---	|
|app   	|Core application (app) code, including models, views, controllers, and helpers   	|
|app/assets   	|Applications assets such as cascading style sheets (CSS), JavaScript files, and images   	|
|bin/ 	|Binary executable files   	|
|config/|Application configuration   	|
|db/   	|Database files   	|
|doc/  	|Documentation for the application   	|
|lib/  	|Library modules   	|
|lib/assets  	|Library assets such as cascading style sheets (CSS), JavaScript files, and images   	|
|log/  	|Application log files   	|
|public/|Data accessible to the public (e.g., via web browsers), such as error pages   	|
|bin/rails  	|A program for generating code, opening console sessions, or starting a local server   	|
|test/ 	|Application tests   	|
|tmp/  	|Temporary files   	|
|Rakefile  	|Utility tasks available via the rake command   	|
|Gemfile  	|Gem requirements for this app   	|
|Gemfile.lock  	|A list of gems used to ensure that all copies of the app use the same gem versions   	|
|config.ru  	|A configuration file for [Rack middleware](http://rack.github.io/)   	|


After creating a new Rails application, the next step is to use Bundler to
install and include the gems needed by the app.
The `bundle install` command might take a few moments, but when it’s done
our application will be ready to run.

If you get the message saying you need to run `bundle update` first, let do 
it.

== Running rails server ==

`rails server` then access from browser: 0.0.0.0:3000
