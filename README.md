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
5. Remove the connection to my Github `git remote remove origin`
6. Create your own repo `gh repo create`

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
To use the gem `middlman-metaman`, [follow these setup instructions](https://github.com/cacheventures/middleman-metaman/)

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
