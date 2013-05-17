desc 'deploys all files'
task :all do
    puts 'deploy all files'
end

desc 'deploys my awesome files'
task :awesome do
    `rm -rf '~/.config/awesome'`
    `cp -r 'awesome' '~/.config/'`
    puts 'awesome deployed'
end

desc 'deploys my bash files'
task :bash do
    `rm '~/.bash_aliases' '~/.bashrc'`
    `cp bash/* ~`
    puts 'bash files deployed'
end

desc 'deploys my conky files'
task :conky do
    puts 'this is a stub'
end

desc 'deploys my vim files'
task :vim do
    `rm -rf '~/.vim' '~/.vimrc'`
    `cp -r 'vim' '~/.vim'`
    `cp 'vim/vimrc' '~/.vimrc'`
    puts 'vim deployed'
end
