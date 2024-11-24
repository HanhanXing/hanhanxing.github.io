# 这是原版国外的源
# source "https://rubygems.org" 
# 这是国内镜像源（快一点）
source "https://gems.ruby-china.com/" 


gem "jekyll", ENV["JEKYLL_VERSION"] if ENV["JEKYLL_VERSION"] # 应该是jekyll 3.10.0 和 4.3.4之间选择，updated in 24-11-21

# 常规：使用 GitHub Pages 默认启用且不能禁用的插件(有一个“github-pages”就行了)。功能：支持 GitHub 风格的 Markdown。建议安装。
# 似乎GitHub-pages这个gem根2.5.1版minima强行绑定了，以至于这里不能整个挪用“group: :jekyll_plugins”
# gem 'github-pages', group: :jekyll_plugins


# 添加以下部份行以明确 Jekyll 插件依赖 (此部份都是跟“gem 'github-pages', group: :jekyll_plugins”里面版本一致的，不一致的都不安装了 )
gem "jekyll-feed", "~> 0.17" #功能：生成站点 RSS 或 Atom 提要。必要性：非必须，只有在需要 RSS 提要时安装。
gem "jekyll-seo-tag", "~> 2.8" # 功能：为站点生成 SEO 元数据。
gem "jekyll-commonmark-ghpages" #(gh默认0.5，但ruby china最新只有0.4)使用 CommonMark 渲染 Markdown，比默认的 kramdown 更现代,必要性：建议安装，特别是对 Markdown 渲染兼容性要求高时。
gem "jekyll-paginate", "~> 1.1.0" #为博客生成分页功能。必要性：建议安装，适用于文章较多的站点。
gem "jekyll-relative-links", "~> 0.6.1" #功能：解析和修正相对链接。必要性：非必须，仅在站点有复杂链接结构时使用。
gem "jekyll-remote-theme", "~> 0.4.3" # 加载远程主题（GitHub 上的主题仓库）。必要性：必要，仅在使用 remote_theme 时安装。
# gem "jekyll-sass-converter", "~> 1.5.2" #功能：将 SASS/SCSS 文件转换为 CSS。必要性：建议安装，尤其是使用自定义样式时。
gem "jekyll-sass-converter", "~> 3.0"
gem "jekyll-sitemap", "~> 1.4.0" # 功能：生成站点的 sitemap（站点地图）。必要性：建议安装，有助于搜索引擎爬取站点。
gem "jekyll-spaceship", "~> 0.10.2" # 功能：增强 Jekyll 的 Markdown 渲染能力。必要性：非必须，仅在需要特殊渲染时安装。

# Markdown 渲染引擎和其他工具
gem "jemoji", "~> 0.13.0" #功能：支持 Emoji 渲染。
gem "kramdown", "~> 2.4" #默认的 Markdown 渲染引擎。
gem "kramdown-parser-gfm" # if ENV["JEKYLL_VERSION"] == "~> 3.9"
gem "nokogiri", "~> 1.16", ">= 1.16.7" #功能：用于解析和操作 HTML/XML。必要性：必要，很多插件依赖它。
gem "rouge", "~> 3.30.0" #功能：用于代码高亮。必要性：建议安装。
gem "safe_yaml", "~> 1.0.5" #功能：解析 YAML 文件。必要性：必须安装。

# 样式相关的工具
gem "liquid", "~> 4.0.4" #功能：Jekyll 使用的模板语言。必要性：必须安装。
gem "sass", "~> 3.7.4" # 功能：SASS/SCSS 样式表支持。必要性：建议安装，尤其是使用 SASS/SCSS 时。


# 明确theme主题使用的路径：minima（3.0onward就用本地的，因为gh pages上是2.5老版本；如果其他主题的话再另说……）
# 各种源里只有最新2.5.1版本的minima，要么remot-theme，要么就直接克隆minima仓库到本地来用
# 1. 这里使用本地路径中的 minima 主题：
# gem 'minima', path: './minima'
# 2. 这里使用remote_theme，先把jekyll-remote-theme插件放上

# gem "jekyll-sass-converter", "~> 3.0" #注意，在jekyll-theme-yat主题的时候，ph pages默认的sass-converter版本就过旧了，要升级到3.0才行
# gem 'jekyll-theme-yat', path: './jekyll-theme-yat' # update in 24-11-20

# Windows does not include zoneinfo files, so bundle the tzinfo-data gem，update in 24-11-20
gem "tzinfo-data", platforms: [:mingw, :mswin, :x64_mingw, :jruby] #，update in 24-11-20
# Performance-booster for watching directories on Windows，update in 24-11-20
gem "wdm", "~> 0.1.0" if Gem.win_platform? #，update in 24-11-20

# 添加 webrick 以避免 LoadError
gem 'webrick', '~> 1.7'