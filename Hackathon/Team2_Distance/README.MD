# Team 2: Distance

Benötigtes Paket 'geosphere'

if (!require('geosphere')) install.packages('geosphere')# to calculate bird flight distance

Die luftlinie funktion verwendet Haversein method 
## Beispiel Funktion 

Variablen:

  source_long: Quell Standort longitude
  
  source_lat: Quell Standort latitude
  
  dest_long: Ziel longitude
  
  dest_lat: Ziel latitude

birdflight_distance <- function(v)
{

	source_long <- v[1]
	
	source_lat  <- v[2]
	
	dest_long   <- v[3]
	
	dest_lat    <- v[4]
	
	dist_km     <- distHaversine(p1 = c(source_long, source_lat)
							 ,p2 = c(dest_long, dest_lat))/1000
							 
	return(dist_km)
	
}
