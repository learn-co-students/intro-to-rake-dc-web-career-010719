desc 'outputs hello to the terminal'

task :environment do
  require_relative './config/environment'
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
  binding.pry
end


namespace :db do
    desc 'migrate changes to your database'
    task :migrate => :environment do
      puts "Hello"
    end
    task :seed do
      require_relative './db/seeds.rb'
    end
    end
    
