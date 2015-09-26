## How To tutorial
1. Install plataformatec's devise 
	* https://github.com/plataformatec/devise
	* Note: required to use default table name of User!!!
2. Copy repo to application
3. Add gem to Gemfile
	* ````gem 'dyalikeblags', path: "path/to/dyalikeblags"```
	* bundle install
4. Add mountpoint to /config/routes.rb
	* mount Dyalikeblags::Engine => "/blog"
	* can change /blog to your preferred path
5. rake db:migrate
	* all migrations should come from within the gem engine

### Usage
1. Access the blog from /blog
2. Access the dashboard from /blog/dashboard/posts

## Notes
* In any dashboard text field full html and bootstrap tags are available.

## To Do
1. Simplify installation using a generator:
-http://multithreaded.stitchfix.com/blog/2014/01/06/rails-app-templates/
1. Categories
2. Pagination or perma scroll or sideways tray?
3. Comments
4. Votable Comments
5. Search
6. Declarative Authorization and user roles/permissions
7. Bring code up to rubocop standards
8. Make install process easier.
6. if time_allows {:implement_testing} else {puts 'lol'}





