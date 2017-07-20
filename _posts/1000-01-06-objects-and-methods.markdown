---
title: Objects and Methods
layout: post
date: 1000-01-06
permalink: objects-and-methods
program: back-end
tags: back-end
---

<h4>What is a Class?</h4>

A class is what is used to define an object that has behavior and attributes. We've already seen built-in classes in Ruby: String, Array, Integer, etc. These classes are all objects with their own behavior and attributes. For example, it wouldn't make sense to call `#capitalize` on an object that has the type "Integer".

<h4>Naming Conventions</h4>

Unlike variable naming, we use CamelCase for naming classes. Here are some examples of how you would create five different classes:

```ruby
class Person
end

class BlogPost
end

class Animal
end

class Task
end

class Car
end
```

The syntax above defines the class. You can think of it as a blueprint. Once you have a blueprint, you can use it to create one, or two, or infinite numbers of the object. Here's an example of defining a `Building` class and then creating three different instances of the Building:

```ruby
class Building
end

hotel = Building.new
office_building = Building.new
school = Building.new
```

<div class="try-it">
<h2>Try It: Defining a Class and Creating Instances</h2>

<p>Use the example above to define an Animal class in irb and create three instances of an animal.</p>
</div>

<h4>Attributes</h4>

Objects generally will have attributes that contain some type of data specific to that instance. These attributes are stored as instance variables (`@attribute`) upon initialization of a new object. Let's look at the example below:

```ruby
class Task
  def initialize(title, status)
    @title       = title
    @status      = status
  end
end

task_one = Task.new("Learn Ruby", "in progress")
```

If you run this file, you won't see anything happen. In order to see the task that you created, you probably want to add the line below. The "p" is kind of like "puts", but it will allow us to not just see the object's ID, but we will also be able to see its attributes. 

```ruby
p task_one
```

<div class="try-it">
<h2>Try It: Defining classes with attributes</h2>

<p>In a new file, create </p>

<pre>4 multiplied by 5 is 20
7 multiplied by 5 is 35
8 multiplied by 5 is 40
12 multiplied by 5 is 60</pre>
Try getting started before looking at the code snippet below. If you're stuck, check out the starter code below:
</div>

We can use these instance variables in any other method that we define in the class.

```ruby
class Task
  attr_reader :title, :status

  def initialize(title, status)
    @title       = title
    @status      = status
  end
end
```

This allows us to do the following:

```ruby
task = Task.new("Buy airplane ticket", "Incomplete")
task.title #=> "Buy airplane ticket"
task.status #=> "Incomplete"
```

<h4>Behavior and Actions</h4>

Behavior of an object is encapsulated in its methods. For example, completing a task would be an action. Asking whether or not the task is complete would also be an action.

```ruby
class Task
  attr_reader   :title, :description
  attr_accessor :status

  def initialize(title, description, status)
    @title       = title
    @description = description
    @status      = status
  end

  def complete!
    @status = "Complete"
  end

  def complete?
    @status == "Complete"
  end
end
```

<h4>Initializing an Object</h4>

Now that we've defined the class, we can create new instances of the object and call its methods:

```ruby
task = Task.new("Buy ticket", "Incomplete")
task.complete? #=> false
task.complete!
task.complete? #=> true
```

<h4>Classes Interacting</h4>

<div class="try-it">
<h2>Try It: Creating the Person Class</h2>

<p>Create a new file called <code>person.rb</code>. A person should have <b>attributes</b> of name, age, and language. Create a method celebrate_birthday! that increases the person's age by one year. The interaction patter should look like the one below. Try out your code and make sure it works!</p>
<pre>kris = Person.new("Kris", 35, "English")
kris.name
"Kris"
kris.language
"English"
kris.age
35
kris.celebrate_birthday!
kris.age
36
</pre>
</div>
