https://jesterjunk.github.io/list_criterion/data.json

    1697 entries

https://jesterjunk.github.io/list_criterion/

https://jesterjunk.github.io/list_criterion/data_entry.html


    counts by first character of titles

    title: "1       3
    title: "2       3
    title: "3       5
    title: "4       4
    title: "7       1
    title: "8       1
    title: ".       1
    title: "A     107
    title: "B      94
    title: "C      69
    title: "D      69
    title: "E      85
    title: "F      51
    title: "G      41
    title: "H      40
    title: "I      61
    title: "J      25
    title: "K      22
    title: "L     117
    title: "M     104
    title: "N      28
    title: "O      32
    title: "P      61
    title: "Q       4
    title: "R      43
    title: "S     104
    title: "T     411
    title: "U      11
    title: "V      18
    title: "W      44
    title: "X       1
    title: "Y       8
    title: "Z      23
    title: "¡       1
    title: "À       3
    title: "Å       1
    title: "’       1
                 1697


### schema reference
```javascript
{
  "entries": [
    {
      "type": "string",                 // "film" or "boxset"
      "url": "string",                  // URL to the Criterion page for the film or boxset
      "slug": "string",                 // Unique identifier slug
      "cover": {
        "artist": "string",             // Name of the cover artist
        "thumbnail": "string",          // URL to the thumbnail image
        "small": "string",              // URL to the small-sized image
        "large": "string",              // URL to the large-sized image
        "original": "string"            // URL to the original-sized image
      },
      "title": "string",                // Title of the film or boxset
      "director": [
        {
          "name": "string",             // Name of the director
          "url": "string"               // URL to the Criterion page for the director
        }
      ],
      "description": "string",          // Description of the film or boxset
      "country": "string",              // Country of origin
      "year": "integer",                // Year of release
      "minutes": "integer",             // Duration in minutes
      "color": "string",                // "Color" or "Black & White"
      "aspect_ratio": "string",         // Aspect ratio
      "language": "string",             // Language of the film
      "spine_number": "integer",        // Criterion spine number
      "purchase_option": [
        {
          "format": "string",           // Format of the purchase option, e.g., "DVD", "BLU-RAY"
          "discs": "string",            // Number of discs
          "srp": "string",              // Suggested retail price
          "oop": "integer"              // Out of print status, 0 for in print, 1 for out of print
        }
      ],
      "external": {
        "imdb": "string",               // URL to IMDb page
        "wikipedia": "string",          // URL to Wikipedia page
        "wikidata": "string",           // URL to Wikidata page
        "icheckmovies": "string",       // URL to ICheckMovies page
        "letterboxd": "string",         // URL to Letterboxd page
        "blu-ray": {
          "dvd": {
            "url": "string",            // URL to Blu-ray.com DVD page
            "release_date": "string"    // Release date for the DVD
          },
          "blu-ray": {
            "url": "string",            // URL to Blu-ray.com Blu-ray page
            "release_date": "string"    // Release date for the Blu-ray
          },
          "blu-ray-4k": {
            "url": "string",            // URL to Blu-ray.com 4K Blu-ray page
            "release_date": "string"    // Release date for the 4K Blu-ray
          }
        }
      },
      "films_in_boxset": [
        "string"                        // URL to each film included in the boxset *
      ]
    }
  ]
}

// "films_in_boxset" is only included if "type" is "boxset"
```
