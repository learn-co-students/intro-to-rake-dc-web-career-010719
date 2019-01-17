desc 'to link the Rakefile to the environment file'
task :environment do
  require_relative './config/environment'
end

namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'outpust hola to the terminal'
  task :hola do
    puts "hola de Rake!"
  end
end

desc 'drop into the Pry console'
task :console => :environment do
  Pry.start
end

namespace :db do
  desc 'migrate changes to database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'seed dummy data into database'
  task :seed do
    require_relative './db/seeds.rb'
  end
end
