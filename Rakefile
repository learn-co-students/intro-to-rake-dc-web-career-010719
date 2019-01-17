desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

namespace :greeting do
  task :hello do
    puts "hello from Rake!"
  end

  task :hola do
    puts "hola de Rake!"
  end
end

task :console do
  Pry.start
end

task :environment do
  require_relative './config/environment'
end

namespace :db do
  task :migrate => :environment do
    puts "migrate"
  end

  task :seed do
    Student.create(name: "Melissa", grade: "10th")
    Student.create(name: "April", grade: "10th")
    Student.create(name: "Luke", grade: "9th")
    Student.create(name: "Devon", grade: "11th")
    Student.create(name: "Sarah", grade: "10th")
  end
end