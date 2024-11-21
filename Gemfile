# 这是原版国外的源
# source "https://rubygems.org" 
# 这是国内镜像源（快一点）
source "https://gems.ruby-china.com/" 


gem "jekyll", ENV["JEKYLL_VERSION"] if ENV["JEKYLL_VERSION"]
gem "kramdown-parser-gfm" # if ENV["JEKYLL_VERSION"] == "~> 3.9"
# GitHub Pages 使用默认启用且不能禁用的插件(有一个“github-pages”就行了)
# 似乎GitHub-pages这个gem根2.5.1版minima强行绑定了。。。
# gem 'github-pages'
# gem 'github-pages', group: :jekyll_plugins


# 添加以下两行以明确依赖
gem "jekyll-feed", "~> 0.17"
gem "jekyll-seo-tag", "~> 2.8"
# 新添加的依赖 - 为了更改主题，update in 24-11-20
gem "jekyll-remote-theme" # ，update in 24-11-20
gem "jekyll-sitemap" # ，update in 24-11-20
gem "jekyll-paginate" # ，update in 24-11-20
gem "jekyll-spaceship" # ，update in 24-11-20

# 各种源里只有最新2.5.1版本的minima，要么remot-theme，要么就直接克隆minima仓库到本地来用
# 使用本地路径中的 minima 主题
# gem 'minima', path: './minima' (# ，update in 24-11-20

# 添加 webrick 以避免 LoadError
gem 'webrick', '~> 1.7'