require "bundler/gem_tasks"

require 'rspec/core/rake_task'

task :default => :spec

desc "Run specs"
RSpec::Core::RakeTask.new

desc "Executes generate on test_repo"
task :generate_test_repo do
  exec 'bundle exec git_stats generate -p spec/integration/test_repo -o test_repo_generate'
end
