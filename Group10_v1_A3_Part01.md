# API description

Our API has a list of birds that can be found in Manitoba.

Our API has pictures of various birds that can live and breed in Manitoba

# List of endpoints with parameters (see below for requirements)
- Endpoints and Parameters: Describe 1-3 endpoints. If you have one endpoint, include at
least 3 parameters. If you have two endpoints, include at least 2 parameters. If you have 3
endpoints, include at least 1 parameter.
- Note: If you want to keep it simple, these endpoints could all be GET methods

# Description of resources - formatted as JSON
- one or two resources

```
class BirdResource

  attributes :name, :breed

  # name setter
  def name=(new_name)
    @model.name = new_name
  end
  
  # breed setter
  def breed=(new_breed)
    @model.breed = new_breed
  end

  # breed getter
  def breed
    @model.breed.to_s
  end
  
  # name getter
  def name
    @model.name.to_s
  end
end
```

# Sample request with sample response

