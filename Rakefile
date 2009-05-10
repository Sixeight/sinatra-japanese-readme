
desc 'Extract Japanese line'
task :default do
  File.open('README.en.rdoc') do |en|
    File.open('README.rdoc', 'wb') do |ja|
      en.readlines.each do |l|
        ja.write l unless /\A#/ =~ l
      end
    end
  end
end

