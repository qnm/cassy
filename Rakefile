#!/usr/bin/env rake

# load rspec so we can set up the environment correctly using spec_helper
require 'rspec/core/rake_task'
require_relative './spec/spec_helper.rb'
RSpec::Core::RakeTask.new(:spec)

Bundler::GemHelper.install_tasks

begin
  require 'bundler/setup'
rescue LoadError
  puts 'You must `gem install bundler` and `bundle install` to run rake tasks'
end

task :default => :spec
