---
layout: post
title:  "Tutorial Membuat VPC di AWS"
date:   2019-10-12 15:28:26 +0700
categories: aws
---
Tutorial kali ini adalah catatan saya pribadi ketika ingin membuat VPC di AWS, apa itu VPC ?. Kalau merujuk dari situs AWS sendiri VPC adalah : Amazon Virtual Private Cloud (Amazon VPC) memungkinkan Anda menyediakan bagian yang terisolasi secara logika pada AWS Cloud di mana Anda dapat meluncurkan sumber daya AWS pada jaringan virtual yang Anda tentukan. 

Intinya kita ingin membuat subnet network sendiri pada instance kita. Disini nanti saya ingin membuat dua topologi subnet, publik subnet dan private subnet, yang mana public subnet nanti ia memiliki ip public sendiri agar ia bisa diakses dari luar jaringan AWS, yang subnet private ia cuman bisa diakses dari server yang berada dalam satu VPC dengannya, jadi tidak memiliki ip public, biasanya digunakan untuk keperluan database server, dsb sesuai kebutuhan. 


Subnet utama : 

10.0.0.0/16

public : 10.0.1.0/24

private : 10.0.2.0/24

![image-title-here](/path/to/image.jpg){:class="img-responsive"}




Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

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
