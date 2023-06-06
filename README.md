# Middleman Template
A simple way to build static pages with a Rails feel.

## Using

- [Middleman](https://middlemanapp.com)
- [Sass](https://sass-lang.com)
- [Bootstrap](https://getbootstrap.com/docs/5.0/getting-started/introduction/)
- [FontAwesome](https://fontawesome.com/icons)

## Init a new project
1. In the repo, click on the green `Code` button to copy your SSH address
2. In Terminal, move to your code folder (or where you want to download the new repo)
3. Clone the repository like this
`git clone git@github.com:dmbf29/middleman-template.git middleman-portfolio`
4. Move into the directory `cd middleman-portfolio`
5. Remove my git history. `rm -rf .git`
6. Start a new git repo in that folder `git init`
7. Create your own repo `gh repo create middleman-portfolio --public --source=.`

### Installation
```
gem install middleman
bundle install
```
⚠️ You may run into some into some gem warnings.<br>
Warnings == 👌, but Fatal errors == ⛔️<br>
If you get a fatal error, you can try fixing it with `bundle update` and hope for the best 🤞

## Run a server
- `middleman`<br>
or if that fails, try
- `bundle exec middleman`

## Deploy
1. [Sign into Netlify](https://www.netlify.com/)
2. Add new site -> Import an existing project -> Github
3. Choose repository and branch
4. Make sure your deploy settings look like this:
<img width="400" alt="Screen Shot 2021-06-18 at 14 19 13" src="https://user-images.githubusercontent.com/25542223/122510271-49d34900-d040-11eb-853f-5105b5d48fcd.png">
5. Website is deployed!
6. (Add purchased domain)

## Meta Tags
You can copy and paste these meta tags inside your `<head></head>` and update the information.
```
<title><%= current_page.data.title || "NAME OF MY SITE | MY TITLE" %></title>
<meta name="description" content="Description of my portfolio site">
<!-- Facebook Open Graph data -->
<meta property="og:title" content="NAME OF MY SITE | MY TITLE" />
<meta property="og:type" content="website" />
<meta property="og:url" content="THE_URL_OF_MY_PORTFOLIO" />
<meta property="og:image" content="<%= image_path 'MY_OG_IMAGE_WITH_RIGHT_SIZE.png' %>" />
<meta property="og:description" content="Description of my portfolio site" />
<meta property="og:site_name" content="NAME OF MY SITE | MY TITLE" />
<!-- Twitter Card data -->
<meta name="twitter:card" content="summary_large_image">
<meta name="twitter:site" content="@twitter_handle">
<meta name="twitter:title" content="NAME OF MY SITE | MY TITLE">
<meta name="twitter:description" content="Description of my portfolio site">
<meta name="twitter:creator" content="@twitter_handle">
<meta name="twitter:image:src" content="<%= image_path 'MY_OG_IMAGE_WITH_RIGHT_SIZE.png' %>">
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
