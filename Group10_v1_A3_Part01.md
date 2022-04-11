# API description

Our API has pictures of various birds that can be found living in Manitoba. This API will be useful for people who enjoy looking at pictures of birds, and for developers who want to incorporate pictures of birds into their applications.


# List of endpoints with parameters
### getRandomBird(location)
 - Returns a random picture of a bird that can be found in a specific location of Manitoba.
### getBirdBySpecies(species)
 - Returns a random picture of a bird belonging to the specified species that can be found in Manitoba.
### getFlyingBird(species)
 - Returns a random picture of a specified flying bird that can be found in Manitoba.
### parameters
 - location (String): the name of city or representative geographic location in Manitoba.
 - species (String): the name of the species of birds. 
# Description of resources

The API has a Bird resource that contains the species, category and location attributes for each bird picture. The species attribute contains the name of the bird species shown in the picture, and the category attribute contains the name of the category of the bird picture. The different categories include pictures of flying birds, pictures of standing birds, and an "other" category for pictures of birds doing other things. The location attribute contains the name of the location where the bird species is most distributed.

```
class BirdResource

  attributes :species, :category, :location

  # species setter
  def species=(new_species)
    @model.species = new_species
  end
  
  # category setter
  def category=(new_category)
    @model.category = new_category
  end
  
  # location setter
  def location=(new_location)
    @model.location = new_location
  end
  
  # species getter
  def species
    @model.species.to_s
  end
  
  # category getter
  def category
    @model.category.to_s
  end
  
  # location getter
  def location
    @model.location.to_s
  end
end
```

# Sample request with sample response
### Sample request
Here is a sample request for a picture of a flying Canada Goose.

```
{
   "species" : "Canada Goose"
   "category": "Flying"
}
```
### Sample response
The API responds with an image of a flying Canada Goose.
```
{
   "image" : "https://upload.wikimedia.org/wikipedia/commons/4/4e/Canada-Goose-Szmurlo.jpg"
}
```


