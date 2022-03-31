source 'https://rubygems.org'

gem 'rails',        '5.1.6'
gem 'puma',         '4.3.12'
gem 'sass-rails',   '5.0.6'
gem 'uglifier',     '3.2.0'
gem 'coffee-rails', '4.2.2'
gem 'jquery-rails', '4.3.1'
gem 'turbolinks',   '5.0.1'
gem 'jbuilder',     '2.7.0'

# 開発かつ、テストの時に使うものを記載
# HerokuではSQLiteがサポートされていないため、リスト 1.5の変更を行って、sqlite3 gemが本番環境に導入されないようにしておきます。
group :development, :test do
  gem 'sqlite3',      '1.3.13'
  gem 'byebug', '9.0.6', platform: :mri
end

# 開発の時に使うものを記載
group :development do
  gem 'web-console',           '3.5.1'
  gem 'listen',                '3.1.5'
  gem 'spring',                '2.0.2'
  gem 'spring-watcher-listen', '2.0.1'
end

# HerokuではPostgreSQLデータベースを使います (ちなみに発音は “post-gres-cue-ell” で、よく“Postgres”と略されます)。そのためには、本番 (production) 環境にpg gemをインストールしてRailsがPostgreSQLと通信できるようにします27 。
group :production do
  gem 'pg', '0.20.0'
end

# Windows環境ではtzinfo-dataというgemを含める必要があります
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]

