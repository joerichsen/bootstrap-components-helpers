## Twitter Bootstrap Components Helper

Provides an `accordion` helper and a `tabs` helper

In your Gemfile:

    gem 'bootstrap-components-helpers', :git => 'git://gist.github.com/2117187.git'

### Accordion helper:
    
    = accordion do |accordion|
      = accordion.pane 'My first pane' do
        = render partial: 'my_first_pane'
      = accordion.pane 'My second pane' do
        = render partial: 'my_second_pane'

`accordion` method options :

  - `:accordion_id` : when you want more than one accordion on the same page
  - `:open` : when you want the first pane to be open on load
  
### Tabs helper:

    = tabs do |tabs|
      - tabs.pane 'My first pane' do
        = render partial: 'my_first_pane'
      - tabs.pane 'My second pane' do
        = render partial: 'my_second_pane'
        
`tabs` method options :

  - `:direction` : to control the positioning of the tabs. Valid values are below, left, right and above (default).