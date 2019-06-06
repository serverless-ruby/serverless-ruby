# serverless-ruby


Blog website [serverless-ruby.org](https://serverless-ruby.org) built with:

* FE framework: [bootstrap 4](https://getbootstrap.com/docs/4.0/)
* static website compiled with [Middleman 4](https://middlemanapp.com/) ([Ruby](https://www.ruby-lang.org/en/))


## Contribution

New articles are welcome. Improvements to the website look are also are welcome.

**please don't commit `/docs` changes** (compiled website changes). Please PR
only changes in `/source` or `/data` folders.

If you never worked with [Middleman](https://middlemanapp.com/) please read https://middlemanapp.com/basics/templating_language/ 


#### Starting website in your laptop (development)


Fork repo, `git clone` fork to your laptop, cd to the folder and do:

```
bundle install
middleman server
```

website will be served on <http://localhost:4567/>


#### tests

no tests are implemented


## Deployment

Deployment can be done only by maintainer of this repo ([Equivalent](https://github.com/equivalent)).

Due to fact the website is hosted on [Github Pages](https://pages.github.com/)
and GH pages supports only Jekyll (not Middleman),
static files needs to be compiled and commited to `/docs` folder.

So **if you are contributing an article / website improvements**
repo maintainer will compile and deploy your article / changes. Pls
don't commit files in `/docs`

Steps for maintainer to deploy:

```
middleman build  #to build soucres to /docs
git add .
git push origin master
```


