---
title: Getting User Input
layout: post
date: 1000-01-05
permalink: getting-user-input
program: back-end
tags: back-end
---

Our program isn't very exciting so far. Let's make a new program called `user_input.rb` and try this out:

```ruby
puts "Enter your name: "
username = gets.chomp
puts "Nice to meet you, #{username}."
```

<div class="try-it">
<h2>Try it: Getting User Input</h2>

<p>Write a program that asks a user for their name, location, and email address. Output the following:</p>

<pre>Your name is Rachel and you live in Las Vegas, NV. Your email address is rachel@girldevelopit.com.</pre>
Try running your program a few times with different inputs.
</div>
