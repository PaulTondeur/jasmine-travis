require 'jasmine'
load 'jasmine/tasks/jasmine.rake'

task :travis do
    system("export DISPLAY=:99.0 && bundle exec rake jasmine:ci")
    raise "rake jasmine:ci failed!" unless $?.exitstatus == 0
end

task :default => "travis"