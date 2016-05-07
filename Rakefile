# -*- ruby -*-

require "rubygems"
require "hoe"

Hoe.plugin :git
Hoe.plugin :gemspec

Hoe.spec "minitest-rails" do
  developer "Mike Moore", "mike@blowmage.com"

  self.summary     = "Minitest integration for Rails"
  self.description = "Adds Minitest as the default testing library in Rails"
  self.urls        = ["http://blowmage.com/minitest-rails"]

  self.history_file = "CHANGELOG.rdoc"
  self.readme_file  = "README.rdoc"
  self.testlib      = :minitest

  license "MIT"

  dependency "minitest",       "~> 5.8"
  dependency "railties",       "~> 5.0.0.rc1"
  dependency "fakefs",         "= 0.4.3", :dev
  dependency "minitest-focus", "~> 1.1", :dev
end

Dir["tasks/**/*.rake"].each { |t| load t }

# vim: syntax=ruby
