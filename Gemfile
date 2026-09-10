source 'https://rubygems.org'

gem 'jekyll'

# The :jekyll_plugins group is auto-loaded by Jekyll whatever `plugins:` in
# _config.yml says, so this list — not that one — is what decides which plugins
# run. Trimmed to the club site: no bibliography, notebooks, archives, remote
# JSON or imagemagick variants, all of which the personal site needs and this
# one does not.
group :jekyll_plugins do
    gem 'jekyll-email-protect'
    gem 'jekyll-link-attributes'
    gem 'jekyll-minifier'
    gem 'jekyll-regex-replace'
    gem 'jekyll-sitemap'
    gem 'jekyll-terser', :git => "https://github.com/RobertoJBeltran/jekyll-terser.git"
    gem 'jemoji'
end

group :other_plugins do
    gem 'css_parser'
end
