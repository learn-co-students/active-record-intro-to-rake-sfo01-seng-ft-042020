  namespace :greeting do

    desc 'outputs hello to the terminal'
    task :hello do
      puts "hello from Rake!"
    end

    desc 'outputs hola to the terminal'
    task :hola do
      puts "hola de Rake!"
    end
  end

  desc 'outputs hello to the terminal'
  task :console do
    binding.pry
  end

  namespace :db do
    desc 'migrate db thing'
    task :migrate => :environment do
      Student.create_table
    end

    desc 'put the stuff yooo'
    task :seed do
      require_relative './db/seeds'
    end
  end

  desc 'initialize environment'
  task :environment do
    require_relative './config/environment'
  end

