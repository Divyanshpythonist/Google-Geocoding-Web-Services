# Google-Geocoding-Web-Services

Geocoding is the process of converting addresses (like "1600 Amphitheatre Parkway, Mountain View, CA") into geographic coordinates (like latitude 37.423021 and longitude -122.083739), which you can use to place markers on a map, or position the map.

Reverse geocoding is the process of converting geographic coordinates into a human-readable address.

Google has an excellent web service that allows us to make use of their large
database of geographic information. We can submit a geographical search string
like “Ann Arbor, MI” to their geocoding API and have Google return its best
guess as to where on a map we might find our search string and tell us about the
landmarks nearby.
The geocoding service is free but rate limited so you cannot make unlimited use of
the API in a commercial application. But if you have some survey data where an
end user has entered a location in a free-format input box, you can use this API
to clean up your data quite nicely.
When you are using a free API like Google’s geocoding API, you need to be respectful
in your use of these resources. If too many people abuse the service, Google might
drop or significantly curtail its free service.
You can read the online documentation for this service, but it is quite simple and
you can even test it using a browser by typing the following URL into your browser:
http://maps.googleapis.com/maps/api/geocode/json?address=Ann+Arbor%2C+MI
Make sure to unwrap the URL and remove any spaces from the URL before pasting
it into your browser.
The following is a simple application to prompt the user for a search string, call
the Google geocoding API, and extract information from the returned JSON.

For more details : 

https://developers.google.com/maps/documentation/geocoding/intro
