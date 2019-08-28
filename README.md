# webtest
Test environment for personal website/portfolio development

## Site Layout and Config

For the `hugo-academic` theme, the modifications for the site are as follows:

* Menus
    * adjusting site menu to my organization in `config/_default/menus.toml`
        * deactivate unused widgets
        * rename `projects` to `feathers` (uses the same layout); create/specify new folder with the same name for path
* Appearance (colours, type, etc)
    * these are modified in `/config/_default/params.toml`
        * colour theme: `ocean`
        * font: `classic`
* _Feathers_ 
    * these are based on the `project` widget
    * they pull content from `/feathers` via `page_type = "feathers"` configuration
    * each post is within it's own subdirectory with the format:
        * create subdirectory for post with the format `content/post/#POST_SLUG#/`
        * `featured.jpg` for the image
        * `index.Rmd` for the content and all YAML (including the post's title, and image width)
