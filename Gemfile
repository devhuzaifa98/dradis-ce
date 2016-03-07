source 'https://rubygems.org'

# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '4.2.5.2'

# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'

# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'

# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.1.0'

# See https://github.com/rails/execjs#readme for more supported runtimes
gem 'therubyracer', platforms: :ruby

gem 'bootstrap-sass', '~> 2.3.2.2'
gem 'font-awesome-sass', '~> 4.3.0'

gem 'jquery-rails'
gem 'jquery-ui-rails'
gem 'jquery-fileupload-rails', '~> 0.3.4'
gem 'jquery-hotkeys-rails'

# Cache-friendly, client-side local time
gem 'local_time'


# Turbolinks makes following links in your web application faster. Read more: https://github.com/rails/turbolinks
gem 'turbolinks'

# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.0'

# bundle exec rake doc:rails generates the API under doc/api.
gem 'sdoc', '~> 0.4.0', group: :doc


# Organize Node tree
gem 'acts_as_tree'

gem 'builder'

gem 'rails_autolink', '~> 1.1'
gem 'thor', '~> 0.18'

# To create/read project packages
gem 'rubyzip', '~> 1.1.0', require: 'zip'

gem 'paper_trail', '~> 4.0.0'
gem 'differ', '~> 0.1.2'

# ------------------------------------------------------ With native extensions
# These require native extensions.
# Ensure Traveling Ruby provides an appropriate version before bumping.
# See:
#   http://traveling-ruby.s3-us-west-2.amazonaws.com/list.html

# Use ActiveModel has_secure_password
# Password digests
gem 'bcrypt',   '3.1.10'

# Required by Rails (uglifier and activesupport)
gem 'json', '1.8.2'

# XML manipulation
gem 'nokogiri', '1.6.5'

# MySQL backend
gem 'mysql2', '0.3.18'

# Textile markup
gem 'RedCloth', '4.2.9', require: 'redcloth'

# SQLite3 DB driver
gem 'sqlite3',  '1.3.10', group: :development

# Use Unicorn as the web server
gem 'unicorn',  '4.9.0', group: :production


# --------------------------------------------------------- Dradis Professional
# Authorisation
gem 'cancancan', '~> 1.10'

# Redis-based background worker
gem 'resque', require: 'resque/status_server'
gem 'resque-status'

# Forms that integrate with Twitter's Bootstrap
gem 'simple_form'

# Word content control filter string parsing
gem 'parslet'

# Word screenshots processing
gem 'image_size', '~> 1.3.0'

# Handle authentication at the Rack level
gem 'warden', '~> 1.2.3'

# Schedule cron jobs
gem 'whenever', require: false



# ------------------------------------------------------------------ Deployment
# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development

group :production do
end


# ----------------------------------------------------- Development and Testing
group :development do
  # Access an IRB console on exception pages or by using <%= console %> in views
  gem 'web-console', '~> 2.0'

  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'

  # Alert on n+1 queries
  gem 'bullet'

  # Cleanup logs from asset entries
  gem 'quiet_assets'

  # manage background workers
  gem 'foreman'
  gem 'rerun'
  # opens ActionMailer messages in the browser
  gem 'letter_opener'
  #gem 'ruby-debug'

  # security
  gem 'brakeman', require: false
  gem 'bundler-audit', require: false
end

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug'

  gem "rspec-rails", "2.14.2"
end

group :test do
  gem 'database_cleaner'
  gem 'factory_girl_rails'#, '~> 4.5.0'
  gem 'capybara', '~> 2.4.4'
  gem 'poltergeist'#, '~> 1.6.0'
  gem 'guard-rspec', require: false
  gem 'shoulda-matchers', '~> 2.8.0'
  gem 'timecop'
end


# =================================================== Other plugins and engines
# = ~  Do not edit this file!! ~ ==============================================
# =============================================================================
#
# See Gemfile.plugins to edit the list of plugins and tool connectors that will
# be loaded by the framework.
#
# Plugins in Gemfile.plugins will be loaded automatically, that's where your
# own plugins should be listed.
#

# Base framework classes required by other plugins
gem 'dradis-plugins',   path: '../dradis-plugins'

plugins_file = 'Gemfile.plugins'
if File.exists?(plugins_file)
  eval(IO.read(plugins_file), binding)
end
