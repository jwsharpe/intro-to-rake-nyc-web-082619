

desc "outputs hello to the terminal"
namespace :greeting do
  desc "outputs hello to the terminal"
  task :hello do
    puts "hello from Rake!"
  end

  desc "outputs hola to the terminal"
  task :hola do
    puts "hola de Rake!"
  end
end

desc "hi"
task :console do
  true
end

task :environment do
  require_relative "./config/environment.rb"
end

namespace :db do
  task :migrate => :environment do
    Student.create_table
  end
  task :seed do
    require_relative "./db/seeds.rb"
  end
end
