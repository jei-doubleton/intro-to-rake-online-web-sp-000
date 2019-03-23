namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  desc 'ouputs goodbye to the terminal'
  task :goodbye do
    puts "goodbye from Rake!"
  end
end

task :environment do
  require_relative './confi/environment'
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end
end
