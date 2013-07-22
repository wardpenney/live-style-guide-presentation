task :build do
  puts '
  ****************

  Starting a server to build your deck!

  1. Keep this terminal open, and
  2. `rake open` in a new terminal. Changes to `deck.md` will automatically be built, just
  3. refresh the page.

  Happy presentation-writing!

  ****************'
  trap('INT') do
    puts "Exiting mdpress..."
    exit 0
  end

  `mdpress -a deck.md -s pivotal`

end

task :open do
  `launchy deck/index.html`
end

task :default => [:build]
