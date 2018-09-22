---
layout: post
title: "Default Jekyll Configuration"
date: "2018-09-11 17:54:16 -0600"
published: true
---

# Defaults in Jekyll configuration

Jekyll's already has a set of configuration defaults. Those defaults are not listed in `_config.yml.`

`_config.yml` is only there to override the defaults or add custom key/value pair.

Adding the default setting to `_config.yml` is a good idea for the beginner as to help them aware of what is going on. Once you get a full understanding of what are the defaults, you don't need to add the defaults.

Here is the following defaults.


```YAML
# Where things are
source              : .
destination         : ./_site
collections_dir     : .
plugins_dir         : _plugins
layouts_dir         : _layouts
data_dir            : _data
includes_dir        : _includes
collections:
  posts:
    output          : true

# Handling Reading
safe                : false
include             : [".htaccess"]
exclude             : ["Gemfile", "Gemfile.lock", "node_modules", "vendor/bundle/", "vendor/cache/", "vendor/gems/", "vendor/ruby/"]
keep_files          : [".git", ".svn"]
encoding            : "utf-8"
markdown_ext        : "markdown,mkdown,mkdn,mkd,md"
strict_front_matter : false

# Filtering Content
show_drafts         : null
limit_posts         : 0
future              : false
unpublished         : false

# Plugins
whitelist           : []
plugins             : []

# Conversion
markdown            : kramdown
highlighter         : rouge
lsi                 : false
excerpt_separator   : "\n\n"
incremental         : false

# Serving
detach              : false
port                : 4000
host                : 127.0.0.1
baseurl             : "" # does not include hostname
show_dir_listing    : false

# Outputting
permalink           : date
paginate_path       : /page:num
timezone            : null

quiet               : false
verbose             : false
defaults            : []

liquid:
  error_mode        : warn
  strict_filters    : false
  strict_variables  : false

# Markdown Processors
rdiscount:
  extensions        : []

redcarpet:
  extensions        : []

kramdown:
  auto_ids          : true
  entity_output     : as_char
  toc_levels        : 1..6
  smart_quotes      : lsquo,rsquo,ldquo,rdquo
  input             : GFM
  hard_wrap         : false
  footnote_nr       : 1
  show_warnings     : false
```
