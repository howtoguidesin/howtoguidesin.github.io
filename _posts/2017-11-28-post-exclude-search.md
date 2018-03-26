---
title: Exclude Post from Search Index
date: 2017-11-28 00:00:00 Z
categories:
- Jekyll
search: false
last_modified_at: 2018-02-19 13:05:00 Z
layout: single
---


    search: false

**Note:** `search: false` only works to exclude posts when using **Lunr** as a search provider.
{: .notice--info}

To exclude files when using ll\\as a search provider add an array to `algolia.files_to_exclude` in your `_config.yml`. For more configuration options be sure to check their [full documentation](https://community.algolia.com/jekyll-algolia/options.html).

    algolia:
      # Exclude more files from indexing
      files_to_exclude:
        - index.html
        - index.md
        - excluded-file.html
        - _posts/2017-11-28-post-exclude-search.md
        - subdirectory/*.html