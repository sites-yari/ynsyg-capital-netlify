---
title:  "Welcome to Jekyll!"
date:   2017-09-13 11:23:47 +0100
categoria: jekyll update
---


You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/


<body class="home page page-id-1512 page-parent page-template page-template-single-page-php">
  <article id="post-3295" class="post-3295 portfolios type-portfolios status-publish hentry">
    <div class="grid" style="padding-top: 80px;">
      <div class="row">

        <div class="c4 imagem-operacao">
          <div class="person-image">
            <img src={{site.data.operacoes.ceriart.img}} alt="Ceriart" />
          </div>
        </div>
        <div class="c8 texto-operacao" style="padding-left: 75px;">
          <h3>{{site.data.operacoes.ceriart.titulo}}</h3>
          <p class="url_empresa"><a href="http://" target="_blank"></a></p>
          <p class="url_empresa"><a href="#" target="_blank"></a></p>
          
          {% for ceriart in site.data.operacoes.ceriart.sobre %} 
            <p class="light-text">
              <b>{{ceriart.topico}}</b><br/>
              {{ceriart.resposta}}
            </p>
          {% endfor %}

        </div>
      </div>
    </div>
  </article>
</body>
