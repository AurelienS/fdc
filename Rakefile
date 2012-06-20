require 'rake/testtask'

Rake::TestTask.new do |t|
  t.libs << 'test'
end

desc "Run tests"
task :default => :test

desc "Launch irb session preloaded with this lib"
task :console do
  sh "irb -rubygems -I lib -r fdc.rb"
end

desc "Launch executable preloaded with this lib and required debug"
task :debug do
  sh "ruby -rubygems -I lib -r debug bin/fdc"
end

desc "Build gem with current .gemspec"
task :build do
  sh "gem build fdc.gemspec"
end