**NOTE:** This codelab is deprecated. See our current codelabs at https://codelabs.developers.google.com/?cat=maps-platform

# Google Maps Web Services Proxy for Mobile Applications
These are the resource files needed for the [Google Maps Web Services Proxy for Mobile Applications](https://codelabs.developers.google.com/codelabs/google-maps-web-services-proxy/)
code lab from Google.

## Introduction for the [Google Maps Web Services Proxy for Mobile Applications](https://codelabs.developers.google.com/codelabs/google-maps-web-services-proxy/)

Suppose you want to create an augmented reality style mobile game, where users must visit real-world locations to progress through the game. Given that a mobile device has access to its current location, the game can randomly generate each location the user needs to visit, but how do you know these locations are accessible? A randomly generated location could very well be in the ocean, or some other inaccessible area.

What you need is a way to identify real-world locations that your game can randomly offer as destinations for the game. The [Google Places API](https://developers.google.com/places/web-service/) is a perfect fit for this, as it allows you to search for places within a particular radius at a given location. Given that the user's mobile device knows its current location, you can use the Google Places API Web Service to search for nearby places, and offer these as destinations the player must reach.

Using the Google Places API directly from a mobile device presents some interesting problems in terms of ensuring API key security, and optimising network performance. This codelab helps you address those issues by building a server-side proxy using [Golang](https://golang.org/) and [Google App Engine](https://cloud.google.com/appengine/). The proxy will take requests from the mobile devices, and make requests to the Google Places API on its behalf.
