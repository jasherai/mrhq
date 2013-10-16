source 'https://rubygems.org'

ruby '1.9.3'

# rails 3.2
#gem 'rails', '~> 3.2.3'
gem 'rails', '~> 3.2.12'
gem 'mysql2'
# Use unicorn as the web server
gem 'unicorn'


# Gems used only for assets and not required
# in production environments by default.

##################### We're not precompiling for a minute
group :assets do
  # See https://github.com/sstephenson/execjs#readme for more supported runtimes
  gem 'therubyracer'

  gem 'coffee-rails', '~> 3.2.1'
  gem 'sass-rails', '~> 3.2.3'
  gem 'uglifier', '>= 1.0.3'

  gem 'jquery-ui-rails'
  gem 'asset_sync'
  gem 'turbo-sprockets-rails3', '~> 0.3.0'
end

group :development, :local_production do
  gem 'yard'
  gem 'foreman'
  gem 'bullet'
  gem 'meta_request'
  gem "binding_of_caller"
  gem 'better_errors'
  gem 'request-log-analyzer'
end

group :development, :local_production, :test do
  gem 'annotate', git: 'git://github.com/ctran/annotate_models.git', require: false
  gem 'railroady'
end


# Global Gems -------------------------------------------------------

gem 'haml'
gem 'coffee-filter'
gem 'cache_digests'
group :local_production, :production, :assets do
  #gem 'themes_for_rails', '~> 0.5.0'
  gem 'themes_for_rails', git: 'git://github.com/jasherai/themes_for_rails.git', branch: 'master'
  #gem 'themes_for_rails', :path => '/home/pmehta/workspace/git-sync.d/themes_for_rails'
end
gem 'jquery-rails'
gem 'devise'
gem 'devise_invitable'
gem 'scoped_roles', git: 'git://github.com/jasherai/scoped_roles.git', branch: :master
#gem 'scoped_roles', :path => '/home/pmehta/workspace/git-sites.d/scoped_roles'
gem "cancan", git: "git://github.com/ryanb/cancan.git", branch: "2.0"
gem 'user_impersonate'
gem 'acts-as-taggable-on'
gem 'awesome_nested_set'
# Edge version but has features we need:
gem 'the_sortable_tree', '>= 1.8.5'
gem 'state_machine'
gem 'mini_exiftool', '>= 2.3.0'
gem 'date_validator'

# Sidekiq and deps
gem 'sinatra', require: nil
gem 'slim'
gem 'sidekiq'
gem 'clockwork'

gem 'transloadit'
gem 'aws-sdk'
gem 'aws-ses', '~> 0.4.4', require: 'aws/ses'
gem 'paperclip'
# Use github source as released gem doesn't handle newrelic instrumentation very well.
gem 'tire-contrib', git: 'git://github.com/karmi/tire-contrib.git'
gem 'tire'
gem 'kaminari'
gem 'make_flaggable', git: 'git://github.com/cavneb/make_flaggable.git'
gem 'rails_config'
gem 'rails3-jquery-autocomplete'
gem 'chronic'
gem "recaptcha", :require => "recaptcha/rails"
gem 'i18n-country-translations'
gem 'i18n_country_select'

# Logging Gems --------------------------------------------------------
gem 'marginalia' #, github: 'carnival/marginalia'
gem 'lograge'

# Instrumentation Gems
group :production do
  gem 'newrelic_rpm'
  gem 'newrelic-redis'
end
gem 'rack-mini-profiler'
gem 'peek', github: 'phatforge/peek'
#gem 'peek-user_impersonate', github: 'phatforge/peek-user_impersonate'
gem 'peek-env_vars'
gem 'peek-gc'
gem 'peek-active_record'
gem 'peek-elasticsearch'
gem 'peek-git'
gem 'peek-mysql2'
gem 'peek-redis'
gem 'peek-performance_bar'
gem 'peek-sidekiq'
# pygments for peek-rblineprof syntax highlighting
gem 'pygments.rb', :require => false
gem 'peek-rblineprof', github: 'phatforge/peek-rblineprof', branch: 'persistence'
gem 'peek-query_reviewer', github: 'peek/peek-query_reviewer'

# Profiling gems
group :profiling do
  gem 'active-profiling'
  gem 'ruby-prof'
  gem 'pilfer'
end

# Error reporting
gem 'airbrake' #, github: 'airbrake/airbrake'
gem 'pinglish'

# Redis Cache/Store etc
gem 'redis-store'
gem 'redis-rails'


# We really should remove the rquirement for this:
gem 'ie_iframe_cookies'
