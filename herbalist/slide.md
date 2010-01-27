!SLIDE bullets incremental
# Herbalist #

* Alchemist (github.com/toastyapps/alchemist)
* Chronic (github.com/evaryont/chronic)

!SLIDE ruby
# Usage of Herbalist #
    
    @@@ ruby
    require 'herbalist'
    
    Herbalist.parse("a quarter cup")
    => #<Alchemist::NumericConversion @value=0.25,
    @exponent=1.0, @unit_name=:cup>

    Herbalist.parse('fifteen kilowatt Hours')
    =>#<Alchemist::NumericConversion @value=15.0,
    @exponent=1.0, @unit_name=:kilowatt_hours>
    
!SLIDE ruby
# Usage #

    @@@ ruby
    require 'herbalist'
    Herbalist.parse("a quarter cup").liters.to_f
    => 0.05914705
    
!SLIDE commandline incremental
# Get It #
    
    $ sudo gem install herbalist
    
!SLIDE commandline incremental
# Help Out #

    $ git clone git://github.com/jduff/herbalist.git
    