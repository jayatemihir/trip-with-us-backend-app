This project implements the backend for TripWithUs application which exposes the following REST APIs to be called via GET HTTP requests:

1. /hotels:
   This API returns the list of all hotels.

2. /hotels/sort/pricing?pricing=<low-to-high/high-tolow>:
   This API returns the list of hotels sorted on the basis of price in the order given by the query parameter 'pricing'.

3. /hotels/sort/rating?rating=<low-to-high/high-tolow>:
   This API returns the list of hotels sorted on the basis of rating in the order given by the query parameter 'rating'.

4. /hotels/sort/reviews?reviews=<low-to-high/high-tolow>:
   This API returns the list of hotels sorted on the basis of reviews in the order given by the query parameter 'reviews'.

5. /hotels/filter/amenity?amenity=<selected amenity>:
   This API returns the list of hotels having the amenity mentioned in the query parameter 'amenity'.

6. /hotels/filter/category?category=<selected category>:
   This API returns the list of hotels belonging to the category mentioned in the query parameter 'category'.

7. /hotels/filter/country?country=<selected country>:
   This API returns the list of hotels situated in the country mentioned in the query parameter 'country'.

Response data will be returned in the following JSON format:
{
    "hotels" : <List of hotels in the result>
}