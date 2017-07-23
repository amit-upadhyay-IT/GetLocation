# GetLocationFast
The fastest ever "displaying users current address" app

To display the users current address I am not using Geocoder class, rather I am using http://maps.googleapis.com/maps/api/geocode/json?latlng=28.600287,77.1171899&sensor=true to fetch the location details.

Using Geocoder is time consuming and also it doesn't always work for all of its methods (atleast in my case).

A special thanks to this library - https://github.com/yayaa/LocationManager , it helped me to achieve this.

In case you get an exception for NotFound LocationRequest, then just add `compile 'com.google.android.gms:play-services-location:10.0.1'` dependency in your `build.gradle`

NOTE: This library uses very very less battery or even no battery in some cases (try it and make your customer happy ).
