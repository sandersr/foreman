# foreman plugins import this file therefore __FILE__ cannot be used
FOREMAN_GEMFILE = __FILE__ unless defined? FOREMAN_GEMFILE

source 'https://rubygems.org'

gem 'rails', '4.1.14.2'
gem 'rest-client', '~> 1.6.0', :require => 'rest_client'
gem 'audited-activerecord', '~> 4.0'
gem 'will_paginate', '~> 3.0'
gem 'ancestry', '~> 2.0'
gem 'scoped_search', '>= 3.2.2', '< 4'
gem 'ldap_fluff', '>= 0.3.5', '< 1.0'
gem 'apipie-rails', '~> 0.3.4'
gem 'rabl', '~> 0.11'
gem 'oauth', '~> 0.4'
gem 'deep_cloneable', '~> 2.0'
gem 'foreigner', '~> 1.4'
gem 'validates_lengths_from_database', '~> 0.5'
gem 'friendly_id', '~> 5.0'
gem 'secure_headers', '~> 1.3'
gem 'safemode', '~> 1.2'
gem 'fast_gettext', '~> 0.8'
gem 'gettext_i18n_rails', '~> 1.0'
gem 'rails-i18n', '~> 4.0.0'
gem 'turbolinks', '~> 2.5'
gem 'logging', '>= 1.8.0', '< 3.0.0'
gem 'fog-core', '1.35.0'
gem 'net-scp'
if RUBY_VERSION.start_with? '1.9.'
  gem 'net-ssh', '< 3'
  gem 'net-ldap', '>= 0.8.0', '< 0.13'
else
  gem 'net-ssh'
  gem 'net-ldap', '>= 0.8.0'
end
gem 'activerecord-session_store', '~> 0.1.1'
gem 'rails-observers', '~> 0.1'
gem 'protected_attributes', '~> 1.1.1'
gem 'sprockets', '~> 3'
gem 'sprockets-rails', '>= 2.3.3', '< 3'

Dir["#{File.dirname(FOREMAN_GEMFILE)}/bundler.d/*.rb"].each do |bundle|
  self.instance_eval(Bundler.read_file(bundle))
end
