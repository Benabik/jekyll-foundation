CONFIGS = %w{_config.yml}

def config
  return '--config ' + CONFIGS.join(',')
end

def jekyll(*args)
  sh 'bundle exec jekyll ' + args.join(' ')
end

desc 'Add asset compression'
task 'compress' do
  CONFIGS << '_config.compress.yml'
end

task 'build' do |t, args|
  jekyll 'build', config, *args
end

task 'serve' do |t, args|
  jekyll 'serve', config, *args
end

task 'doctor' do
  jekyll 'doctor'
end

task :default => 'build'
