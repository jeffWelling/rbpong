task :test , [:load_dir] do |t,args|
  $: << File.dirname(File.expand_path(__FILE__))+"/"
  require "rubygems"
  require "rubygame"
  require "test/unit"
  require "test/test.rb"
  include Rubygame
  TTF.setup
  args.with_defaults(:load_dir => "all")
  if args.load_dir == "all"
    all()
  else
    load(args.load_dir)
  end
end
  
