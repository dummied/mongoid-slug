require 'rspec/core/rake_task'
require 'jeweler'

task :default => :spec

desc "Run all specs in spec directory"
RSpec::Core::RakeTask.new(:spec) do |spec|
  spec.pattern = "spec/**/*_spec.rb"
end
  
Jeweler::Tasks.new do |gemspec|
  gemspec.name = "mongoid_slug"
  gemspec.summary = "Generates a URL slug in a Mongoid model"
  gemspec.description = "Mongoid Slug generates a URL slug/permalink based on fields in a Mongoid model."
  gemspec.add_dependency("mongoid", ["~> 2.4.9"])
  gemspec.files = Dir.glob("lib/**/*") + %w(LICENSE README.rdoc)
  gemspec.require_path = 'lib'
  gemspec.email = "code@papercavalier.com"
  gemspec.homepage = "http://github.com/papercavalier/mongoid-slug"
  gemspec.authors = ["Hakan Ensari", "Gerhard Lazu"]
end
Jeweler::GemcutterTasks.new
