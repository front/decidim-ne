# frozen_string_literal: true

source "https://rubygems.org"

ruby RUBY_VERSION

DECIDIM_VERSION = { git: "https://github.com/decidim/decidim", branch: "release/0.24-stable" }

gem "decidim", DECIDIM_VERSION

gem 'decidim-admin', DECIDIM_VERSION
gem 'decidim-blogs', DECIDIM_VERSION
# gem "decidim-consultations", DECIDIM_VERSION
gem "decidim-initiatives", DECIDIM_VERSION
gem "decidim-pages", DECIDIM_VERSION
gem "decidim-proposals", DECIDIM_VERSION
# gem "decidim-templates", DECIDIM_VERSION

# Module that provides a new verification method that allows system
# administrators to define new verification workflows where the admins
# can provide access to specific users.
gem "decidim-access_requests", git: "https://github.com/front/decidim-module-access_requests"

gem "bootsnap", "~> 1.4"

gem "puma", ">= 5.0"
gem "uglifier", "~> 4.1"

gem "faker", "~> 2.14"

gem "wicked_pdf", "~> 1.4"

gem "fog-aws"
gem "aws-sdk"

group :development, :test do
  gem "byebug", "~> 11.0", platform: :mri

  gem "decidim-dev", DECIDIM_VERSION
end

group :development do
  gem "letter_opener_web", "~> 1.3"
  gem "listen", "~> 3.1"
  gem "spring", "~> 2.0"
  gem "spring-watcher-listen", "~> 2.0"
  gem "web-console", "~> 3.5"
end
