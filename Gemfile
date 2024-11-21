# 这是原版国外的源
# source "https://rubygems.org" 
# 这是国内镜像源（快一点）
source "https://gems.ruby-china.com/" 


gem "jekyll", ENV["JEKYLL_VERSION"] if ENV["JEKYLL_VERSION"] # installing jekyll 3.10.0 (was 4.3.4)，updated in 24-11-21
gem "kramdown-parser-gfm" # if ENV["JEKYLL_VERSION"] == "~> 3.9"
# GitHub Pages 使用默认启用且不能禁用的插件(有一个“github-pages”就行了)
# 似乎GitHub-pages这个gem根2.5.1版minima强行绑定了。。。
# gem 'github-pages'
# gem 'github-pages', group: :jekyll_plugins


# 添加以下部份行以明确依赖
gem "jekyll-feed", "~> 0.17"
gem "jekyll-seo-tag", "~> 2.8"
# 新添加的依赖 - 为了更改主题，update in 24-11-20
gem "jekyll-sitemap", "~> 1.4" # ，update in 24-11-20
gem "jekyll-paginate" # ，update in 24-11-20
gem "jekyll-spaceship" # ，update in 24-11-20

# 明确theme主题使用的路径：minima（3.0onward就用本地的，因为gh pages上是2.5老版本；如果其他主题的话再另说……）
# 各种源里只有最新2.5.1版本的minima，要么remot-theme，要么就直接克隆minima仓库到本地来用
# 1. 这里使用本地路径中的 minima 主题：
# gem 'minima', path: './minima' (# ，update in 24-11-20
# 2. 这里使用remote_theme，先把jekyll-remote-theme插件放上（？
gem "jekyll-remote-theme", "~> 0.4.3" # ，update in 24-11-20
# 2.1. 这里用remote theme的时候，gh pages默认的sass-converter版本是旧的，是不是这里也要统一一下本地的？还是说指定一个新版本给线上的？
# gem "jekyll-sass-converter", "~> 1.5.2" 这个不得行哈
gem "jekyll-sass-converter", "~> 3.0"

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem，update in 24-11-20
gem "tzinfo-data", platforms: [:mingw, :mswin, :x64_mingw, :jruby] #，update in 24-11-20
# Performance-booster for watching directories on Windows，update in 24-11-20
gem "wdm", "~> 0.1.0" if Gem.win_platform? #，update in 24-11-20

# 添加 webrick 以避免 LoadError
gem 'webrick', '~> 1.7'