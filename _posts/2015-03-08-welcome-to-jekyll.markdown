---
layout: post
title:  "Welcome to Jekyll!"
date:   2015-03-08 12:00:00
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby linenos=true %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

```javascript

var sp = "Samar Panda";
console.log(sp);

```

```ruby mark:2-4 title:"Testing codefence" url:"https://github.com/octopress/codefence" link_text:"plugin link"
class Float
  def number_decimal_places
    self.to_s.length-2
  end

  def to_fraction
    higher = 10**self.number_decimal_places
    lower = self*higher

    gcden = greatest_common_divisor(higher, lower)

    return (lower/gcden).round, (higher/gcden).round
  end

private

  def greatest_common_divisor(a, b)
     while a%b != 0
       a,b = b.round,(a%b).round
     end 
     return b
  end
end
```

```javascript title:"Testing codefence" url:"https://github.com/octopress/codefence" link_text:"plugin link"
var sp = "Samar Panda";
console.log(sp);
```

{% codeblock lang:js %}

var inorder = function* inorder(node) {
  if (node) {
    yield* inorder(node.left);
    yield node.label;
    yield* inorder(node.right);
  }
}

{% endcodeblock %}


{% codeblock lang:js %}
var arr1 = new Array(arrayLength);
var arr2 = new Array(element0, element1, ..., elementN);
{% endcodeblock %}


{% codeblock lang:ruby start:1 %}
class Fixnum
  def prime?
    ('1' * self) !~ /^1?$|^(11+?)\1+$/
  end
end
{% endcodeblock %}


Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
