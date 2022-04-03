# API description

Our API has pictures of various birds that can live and breed in Manitoba. This API will be useful for people who enjoy looking at pictures of birds, and for developers who want to incorporate pictures of birds into their applications.

# List of endpoints with parameters
### getRandomBird()
 - Returns a random picture of a bird that can be found in Manitoba.
### getBirdBySpecies(species)
 - Returns a random picture of a bird belonging to the specified species that can be found in Manitoba.
### getFlyingBird()
 - Returns a random picture of a flying bird that can be found in Manitoba.

# Description of resources

The API has a Bird resource that contains the species and category attributes for each bird picture. The species attribute contains the name of the bird species shown in the picture, and the category attribute contains the name of the category of the bird picture. The different categories include pictures of flying birds, pictures of standing birds, and an "other" category for pictures of birds doing other things.

```
class BirdResource

  attributes :species, :category

  # species setter
  def species=(new_species)
    @model.species = new_species
  end
  
  # category setter
  def category=(new_category)
    @model.category = new_category
  end

  # species getter
  def species
    @model.species.to_s
  end
  
  # category getter
  def category
    @model.category.to_s
  end
end
```

# Sample request with sample response
### Sample request
```
{
   "species" : "Green-winged teal"
}
```
### Sample response
```
{
   "image" : "https://upload.wikimedia.org/wikipedia/commons/0/07/Green-winged_Teal%2C_Port_Aransas%2C_Texas.jpg"
}
```
