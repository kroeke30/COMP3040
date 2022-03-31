# API description

Our API has pictures of various birds that can live and breed in Manitoba

# List of endpoints with parameters (see below for requirements)
### getRandomBird()
 - Returns a random picture of a bird that can be found in Manitoba.
### getBirdBySpecies(species)
 - Returns a random picture of a bird belong to the specified species that can be found in Manitoba.
### getFlyingBird()
 - Returns a random picture of a flying bird that can be found in Manitoba.

# Description of resources - formatted as JSON
- one or two resources
- brief description overview (to managers)

```
class BirdResource

  attributes :name, :species

  # name setter
  def name=(new_name)
    @model.name = new_name
  end
  
  # species setter
  def species=(new_species)
    @model.species = new_species
  end

  # species getter
  def species
    @model.species.to_s
  end
  
  # name getter
  def name
    @model.name.to_s
  end
end
```

# Sample request with sample response

