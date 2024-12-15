# frozen_string_literal: true

source "https://rubygems.org"
gemspec

rails_version = (ENV["RAILS_VERSION"] || "~> 7.0.0").to_s

gem "capybara", "~> 3"
gem "rails", ">= 7.0.8.7", rails_version == "main" ? {git: "https://github.com/rails/rails", ref: "main"} : rails_version

gem "rspec-rails", "~> 5"

if RUBY_VERSION >= "3.1"
  gem "net-imap", require: false
  gem "net-pop", require: false
  gem "net-smtp", require: false
end
