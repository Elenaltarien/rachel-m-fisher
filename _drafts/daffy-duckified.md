---
layout: post
title: "Beyond Codecademy: Thith Meanth War!"
summary: Expanding on the Codecademy Thith Meanth War! project by adding an until loop.
tags: [coding, Ruby]
---


Codecademy's Tutorial
~~~ruby
puts "Type something:"
user_input = gets.chomp
user_input.downcase!

if user_input.include? "s"
  user_input.gsub!(/s/, "th")
  puts "You've been Daffy Duckified: #{user_input}."
else
  print "There is no s in there."
end
~~~

My program so far
~~~ruby
prompt = "Enter a string to be Daffy Duckified:"
puts prompt
user_input = gets.chomp
user_input.downcase!

until user_input.include? "s"
  if user_input == ""
    puts "You didn't enter anything. Try again."
    puts prompt
  else 
    puts "You didn't have any s' in your string, try again."
    puts prompt
  end
  user_input = gets.chomp
  user_input.downcase!
end

user_input.gsub!(/s/, "th")
puts "Here's your Daffy Duckified string: #{user_input}."
~~~