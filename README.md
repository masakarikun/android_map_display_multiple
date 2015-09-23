# android_map_display_multiple
created to display google map at mutiple(this app shows four maps in a app) see the URL below .
URL:http://androidtechs.jimdo.com/

for activate,
1. put your api key
2. dupulicate below code, the number you want to show.
SupportMapFragment supportMapFragment = (SupportMapFragment) getSupportFragmentManager()
				.findFragmentById(R.id.map);
		googleMap = supportMapFragment.getMap();
		if (googleMap != null) {
			googleMap.addMarker(new MarkerOptions().position(new LatLng(0, 0)).title("現在位置"));
			googleMap.moveCamera(CameraUpdateFactory.newLatLngZoom(latlng, 15));
			googleMap.addMarker(new MarkerOptions().position(latlng).title("現在位置"));

3. change the fragment that shows in the code.
