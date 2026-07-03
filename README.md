# D&D-Linkify-SuttaCentral-IDs
Converts SuttaCentral.net text citations to links

# Development

Clone the repo

# Testing

1. Log into [Discourse Theme Creator](https://discourse.theme-creator.io/) using your [meta.discourse.org](https://meta.discourse.org) account.
2. Click on [My Themes](https://discourse.theme-creator.io/my/themes) in the sidebar
3. Click `Install` > `From a git repository`
4. Get the repo url from the repository by going to `Code` > `Local` > `HTTPS` and copying the url
5. If there is more than one branch, click `Advanced` and enter the branch name.
6. Click `Install`
7. This should take you to the component's edit page. Go to the very bottom and click on `Preview`
8. NOTE: Only pages you visit using this preivew tab will have the component active.
9. Create a new post using the contents of [test-post.md](test-post.md).
10. If everything is successful all the citations that are not ~~struck through~~ should link properly to suttacentral.net

# Adding new citation patterns

1. All new regex patterns should be added to the [settings.yml](settings.yml) file. CAUTION: YAML files are very fussy with proper spacing. If things are failing, be sure to run your new text through an online [YAML parser](https://yamlchecker.com/)
2. Under [My Themes](https://discourse.theme-creator.io/my/themes) click on `Check for Updates`