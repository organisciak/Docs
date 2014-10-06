# `jsoncatalog.txt`

The input for the `jsoncatalog.txt` file contains one JSON object per line. The keys represent shared metadata for each file: the values represent the entry for that particular document. There should be no new line or tab characters in this file.

In addition to the metadata you choose, two fields are required:

1. A `searchstring` field that contains valid HTML which will be served to the user to identify the text. This can be a link, or simply a description of the field.
    * If you have a URL where the text can be read, it's best to include it inside an `<a>` tag: that lets users actually read the text, which is kind of the point here.
    * If the texts are very small (less than a paragraph apiece, say), you might just paste the entire text into the searchstring so users can read them on the search.
    * Otherwise, you can just put in any text field you want in the process of creating the jsoncatalog.txt file: something like author and title is good.

2. A `filename` field that includes a unique identifier for the document (linked to the filename or the identifier, depending on your input format).

Here is an example of the first six items in the Open Library jsoncatalog.txt. Note that the searchstring is valid html; that the "publishers" field is an array:

``` {js}
{"publishers": ["Simon & Schuster Books for Young Readers"], "searchstring": "[No author], <em>Ernestine & Amanda, summer camp ready or not!</em> (undated) <a href=\"http://openlibrary.org/books/OL1002147M\">more info</a> <a href=\"http://archive.org/stream/ernestineamandas00belt\">read</a>", "lc2": "7", "lc0": "P", "title": "Ernestine & Amanda, summer camp ready or not!", "lccn": ["96041443"], "lc1": "PZ", "editionid": "/books/OL1002147M", "publish": 1997, "filename": "er/ne/ernestineamandas00belt", "languages": ["/languages/eng"], "lc_classifications": ["PZ7.B4197 Er 1997"], "publish_date": "1997", "publish_country": "nyu", "key": "/books/OL1002147M", "authors": ["/authors/OL24054A"], "ocaid": "ernestineamandas00belt", "oclc_numbers": ["35360730"], "works": ["/works/OL16070305W"], "publish_places": ["New York"]}
{"publishers": ["Copernicus"], "searchstring": "[No author], <em>The call of distant mammoths</em> (undated) <a href=\"http://openlibrary.org/books/OL1008703M\">more info</a> <a href=\"http://archive.org/stream/callofdistantmam00ward\">read</a>", "lc2": "882", "lc0": "Q", "title": "The call of distant mammoths", "lccn": ["96048690"], "lc1": "QE", "editionid": "/books/OL1008703M", "publish": 1997, "filename": "ca/ll/callofdistantmam00ward", "languages": ["/languages/eng"], "lc_classifications": ["QE882.P8 W37 1997"], "publish_date": "1997", "publish_country": "nyu", "key": "/books/OL1008703M", "authors": ["/authors/OL224736A"], "ocaid": "callofdistantmam00ward", "publish_places": ["New York"], "works": ["/works/OL1876772W"]}
{"publishers": ["Children's Press"], "searchstring": "[No author], <em>Qatar</em> (undated) <a href=\"http://openlibrary.org/books/OL1009559M\">more info</a> <a href=\"http://archive.org/stream/qataraugu00augu\">read</a>", "lc2": "247", "lc0": "D", "title": "Qatar", "lccn": ["96049593"], "lc1": "DS", "editionid": "/books/OL1009559M", "publish": 1997, "filename": "qa/ta/qataraugu00augu", "languages": ["/languages/eng"], "lc_classifications": ["DS247.Q3 A94 1997"], "publish_date": "1997", "publish_country": "nyu", "key": "/books/OL1009559M", "authors": ["/authors/OL544559A"], "ocaid": "qataraugu00augu", "oclc_numbers": ["36008545"], "works": ["/works/OL3353201W"], "publish_places": ["New York"]}
{"publishers": ["New York University Press"], "searchstring": "[No author], <em>Hypertext</em> (undated) <a href=\"http://openlibrary.org/books/OL1009928M\">more info</a> <a href=\"http://archive.org/stream/hypertextelectro00snyd\">read</a>", "lc2": "76", "lc0": "Q", "title": "Hypertext", "lccn": ["96049982"], "lc1": "QA", "editionid": "/books/OL1009928M", "publish": 1997, "filename": "hy/pe/hypertextelectro00snyd", "languages": ["/languages/eng"], "lc_classifications": ["QA76.76.H94 S64 1997"], "publish_date": "1997", "publish_country": "nyu", "key": "/books/OL1009928M", "authors": ["/authors/OL355369A"], "ocaid": "hypertextelectro00snyd", "publish_places": ["New York, N.Y"], "works": ["/works/OL2521051W"]}
{"publishers": ["New Press"], "searchstring": "[No author], <em>The war on the poor</em> (undated) <a href=\"http://openlibrary.org/books/OL1014980M\">more info</a> <a href=\"http://archive.org/stream/waronpoordefense00albe\">read</a>", "lc2": "95", "lc0": "H", "title": "The war on the poor", "lccn": ["96067176"], "lc1": "HV", "editionid": "/books/OL1014980M", "publish": 1996, "filename": "wa/ro/waronpoordefense00albe", "languages": ["/languages/eng"], "lc_classifications": ["HV95 .A599 1996"], "publish_date": "1996", "publish_country": "nyu", "key": "/books/OL1014980M", "authors": ["/authors/OL372071A"], "ocaid": "waronpoordefense00albe", "publish_places": ["New York"], "works": ["/works/OL2591929W"]}
```