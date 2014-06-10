pagination
==========

Instant Pagination

Installation

Add this line to your application's Gemfile:

gem 'instant_pagination'
And then execute:

$ bundle
Or install it yourself as:

$ gem install instant_pagination

Usage

This gem displays pagination in a view. once you install this gem, you get a helper method called as "pagination_links". All you need to do is pass total number of records count, per page pagination count and start count and additional params can be added inside this method as arguments and it will display the pagination in the view.
All you need to do is add a partial for pagination and call the method as mentioned as above.
U can call n numbers of pagination in a single page.
For example : top_pagination and bottom pagination

<%= pagination_links(@total_count, 10, start, params).html_safe %>


