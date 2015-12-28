---
layout: post
title:  "Welcome to Jekyll!"
date:   2015-12-28 17:16:54 +0530
categories: jekyll update
---
Differnt types of datatypes?

Booleans , Symbols ,Numbers ,Strings, Arrays, Hashes

Super() in ruby?

Super() allows  to re-use behaviour that exists in a superclass, then modify to suit the needs of the subclass.Ruby uses the super keyword to call the overriding method. Using super will call the same method, but as defined in the superclass and give you the result.

Difference between class and module in ruby?

A Module is a collection of methods and constants. Superclass of module is object and class is module. Class can be instantiated whereas module cannot.Class inherits behaviour and can  be base for inheritance but in case of module no inheritance

How module can be require?? example?

If a third program wants to use any defined module, it can simply load the module files using the Ruby require statementeg.require 'trig.rb'
require 'moral'y = Trig.sin(Trig::PI/4)
wrongdoing = Moral.sin(Moral::VERY_BAD)3.

What is the difference between validate and validates?

validates is used for built in validations like validates :name, length: { minimum: 2 }
While validate is used for custom validations like:
validate :some_validation
def some_validation
  if found_error
       self.errors.add #...
  end
end

How to load excel file into rails? What is mime tab?

provide an xls file that will open in Excel by default. To do this we'll need to add a new MIME type for xls files and we do this in the mime_types initializer file.
/config/initializers/mime_types.rb
Mime::Type.register "application/xls", :xls

How module can be require?with example?

Require in module can extension along with a file name.

Consider following module written in support.rb file.
module Week
  FIRST_DAY = "Sunday"
  def Week.weeks_in_month
     puts "You have four weeks in a month"
  end
  def Week.weeks_in_year
     puts "You have 52 weeks in a year"
  end
end
Now, you can include this module in a class as follows:
#!/usr/bin/ruby
$LOAD_PATH << '.'
require "support"

class Decade
include Week
  no_of_yrs=10
  def no_of_months
     puts Week::FIRST_DAY
     number=10*12
     puts number
  end
end
d1=Decade.new
puts Week::FIRST_DAY
Week.weeks_in_month
Week.weeks_in_year
d1.no_of_months

Difference between attribute_accessor and attribute_accessible?

attr_accessor creates the getter method.attribute and setter method.attribute= for the specified attributes.
attr_accessible specifies a white list of model attributes that can be set via mass-assignment, such as new(attributes), update_attributes(attributes), or attributes=(attributes)

What is superadmin?

Superadmin has end-end previlages. Superadmin can create/destroy admins. Every application has a Admin/SuperAdmin panel. This SuperAdmin manages one or multiple admins under it. SuperAdmin can access control of admins to different sections of site and the person has access to all managing power.