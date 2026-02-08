# Spellbound 🪄✨- Nandan Praveen, Bornini Chandra, Matyas Beyene

## Inspiration
We observed that university students often struggle to maintain concentration amidst digital distractions and the monotony of prolonged study sessions. Drawing from the principles of gamification, we sought to transform the University of Georgia campus into an interactive landscape where academic effort translates into tangible virtual progress. Our goal was to incentivize physical presence at designated learning centers by rewarding users with unlockable content and a sense of magical progression. 

## What It Does
Spellbound acts as a location-aware productivity companion that restricts focus sessions to verified academic environments such as the Zell Miller Learning Center or Main Library. The application tracks the user's geofenced position in real time to ensure they remain onsite while accumulating focus minutes to advance their level. As users dedicate more time to their studies, they unlock collectible wizard avatars, dynamic video backgrounds, and expanded map locations. 

## How We Built It
We developed the mobile application using the Flutter framework to ensure a responsive and visually engaging cross-platform experience.  
- Core location logic uses the `geolocator` package for precise GPS tracking.   
- `flutter_map` renders interactive OpenStreetMap layers of the Athens campus. 
- The Google Calendar API synchronizes and displays upcoming academic deadlines in the user's quest log.  
- Google's Gemini model assisted in building the application.   

## Challenges We Ran Into
- Managing state synchronization between the home interface and the location module to ensure unlocked rewards persisted correctly across screens.   
- Obtaining precise GPS coordinates for specific buildings like the Science Learning Center, which initially resulted in inaccurate geofencing.   
- Implementing a proximity check that monitored the user's distance from multiple unlockable nodes without draining the battery required careful optimization. 
