require "capistrano/setup"
require "capistrano/deploy"

require "capistrano/scm/git"
install_plugin Capistrano::SCM::Git

# require "capistrano/rbenv"
require "capistrano/bundler"
require "capistrano/rails/assets"
require "capistrano/rails/migrations"
require "capistrano/passenger"
require 'capistrano/yarn'
require 'capistrano/puma'
require 'capistrano/puma/nginx'

install_plugin Capistrano::Puma, load_hooks: true
Dir.glob("lib/capistrano/tasks/*.rake").each { |r| import r }
