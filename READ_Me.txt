Our project uses various methods and structures including the KDTree and dijkstras culminating in a method called
best_route(source,target) which takes in a source coordinate set and target coordinate set representing
a travellers start and end points. The best_route(s,t) method plots these points, uses a KDTree to find the nearest
bus stops to each, and plots a Networkx graph with the route nodes and edges colored. The stops are taken from 
the file "stops.txt" and the edges are created using "trip_id"'s from "stop_times.txt". The time it takes for a bus
to travel from stop to stop is calculated using departure times in "stop_times.txt" and are saved as edge attributes.
Additionally, the method calculates walking time from the source to target and prints this in comparison to the 
time the route would take by transit. We also added a fun little visualizer called color_dist_from_point(ids) 
which takes a "stop_id" and colors surrounding nodes based on their distance from the chosen id. If you would like 
to use this method, you can input any stop_id from the "stops.txt" file. 