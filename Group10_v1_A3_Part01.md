# API description

Our API has pictures of various birds that can live and breed in Manitoba

# List of endpoints with parameters (see below for requirements)
- Endpoints and Parameters: Describe 1-3 endpoints. If you have one endpoint, include at
least 3 parameters. If you have two endpoints, include at least 2 parameters. If you have 3
endpoints, include at least 1 parameter.
- Note: If you want to keep it simple, these endpoints could all be GET methods

 - getRandomBird()
 - getBirdBySpecies(species)
 - getFlyingBird()

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

