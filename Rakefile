# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://docs.rubygems.org/read/chapter/20 for more options
  gem.name = "encrypted_id"
  gem.homepage = "http://github.com/pencil/encrypted_id"
  gem.license = "MIT"
  gem.summary = "Allows you to encrypt the ID of your ActiveRecord model."
  gem.description = "Sometimes you don't want your users to see the actual ID of your databases entries. This gem allows you to hide the ID."
  gem.email = "ncaspar@me.com"
  gem.authors = ["Nils Caspar"]
  # dependencies defined in Gemfile
end
Jeweler::RubygemsDotOrgTasks.new

require 'rspec/core'
require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = FileList['spec/**/*_spec.rb']
end

task :default => :spec
