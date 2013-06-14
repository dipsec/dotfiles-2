desc 'deploys all files'
task :all do
    Rake::Task['awesome'].execute
    Rake::Task['bash'].execute
    Rake::Task['conky'].execute
    Rake::Task['fonts'].execute
    Rake::Task['git'].execute
    Rake::Task['vim:all'].execute
end

desc 'deploys my awesome files'
task :awesome do
    `rm -rf ~/.config/awesome`
    `cp -r awesome ~/.config/`
    puts 'awesome deployed'
end

desc 'deploys my bash files'
task :bash do
    `rm ~/.bash_aliases ~/.bashrc`
    `cp bash/bash_aliases ~/.bash_aliases`
    `cp bash/bashrc ~/.bashrc`
    puts 'bash files deployed'
end

desc 'deploys my conky files'
task :conky do
    puts 'this is a stub'
end

desc 'deploys my custom fonts'
task :fonts do
    `rm -rf ~/.fonts`
    `mkdir ~/.fonts`
    `cp fonts/* ~/.fonts/`
    puts 'fonts deployed'
end

desc 'deploys my git files'
task :git do
    `rm  ~/.gitconfig`
    `cp git/gitconfig ~/.gitconfig`
    puts 'git deployed'
end

namespace :vim do
    desc 'deploys my vim files'

    #task :all do
        #`rm -rf ~/.vim ~/.vimrc`
        #`cp -r vim ~/.vim`
        #`cp vim/vimrc ~/.vimrc`
        #puts 'vim deployed'
    #end

    task :install do
        `vim +BundleInstall +qall > /dev/null 2>&1`
        puts 'Vundle bundles installed'
    end

    desc 'deploys my .vimrc only'
    task :vimrc do
        `rm -rf ~/.vimrc`
        `cp vim/vimrc ~/.vimrc`
        puts '.vimrc deployed'
    end
end

