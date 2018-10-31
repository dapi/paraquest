require 'rubygems'
require 'bundler'
Bundler.setup(:deploy)

require_relative 'app/models/settings'
require_relative 'app/models/app_version'

# Load DSL and Setup Up Stages
require 'capistrano/setup'

# Includes default deployment tasks
require 'capistrano/deploy'

require 'capistrano/scm/git'
install_plugin Capistrano::SCM::Git

require 'capistrano/scm/git-with-submodules'
install_plugin Capistrano::SCM::Git::WithSubmodules

require 'capistrano/master_key'
require 'capistrano/rbenv'
require 'capistrano/bundler'
require 'capistrano-db-tasks'
require 'capistrano/maintenance'
require 'capistrano/shell'
require 'capistrano/puma'
install_plugin Capistrano::Puma
require 'capistrano/rails/assets'
require 'capistrano/faster_assets'
require 'capistrano/rails/migrations'
require 'bugsnag-capistrano'
require 'capistrano/semver-tag'
require 'capistrano/upload-config'

require 'capistrano/tasks'
require 'capistrano/rails/console'
