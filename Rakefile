def jekyll(*args)
  sh 'bundle exec jekyll ' + args.join(' ')
end

task 'build' do |t, args|
  jekyll 'build', *args
end

task 'serve' do |t, args|
  jekyll 'serve', *args
end

task 'doctor' do
  jekyll 'doctor'
end

task :default => 'build'
