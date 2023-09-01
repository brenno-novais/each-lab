require_relative "config/application"
require 'rubygems'
require 'cucumber'
require 'cucumber/rake/task'
require 'rake'
require 'rspec/core/rake_task'
require 'coveralls'

Rails.application.load_tasks

RSpec::Core::RakeTask.new(:spec) 
task :default  => :spec

Cucumber::Rake::Task.new(:features) do |t|
  t.cucumber_opts = ["--format pretty"]
end

Coveralls.wear_merged!('rails')