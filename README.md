# Dijkstra
Method Dijkstra(G, s): // G is graph, s is source  
distance[s] -> 0               // Distance from the source to source is always 0  
for every vertex vx in the Graph G: // doing the initialization work  
{  
if vx ? s  
{  
// Unknown distance function from source to each node set to infinity  
distance[vx] -> infinity   
}  
add vx to Queue Q   // Initially, all the nodes are in Q  
}  
  
// The while loop  
Untill the Q is not empty:                    
{  
// During the first run, this vertex is the source or starting node  
vx = vertex in Q with the minimum distance[vx]   
delete vx from Q   
}  
// where the neighbor ux has not been deleted yet from Q.  
for each neighbor ux of vx:             
              alt = distance[vx] + length(vx, ux)  
              // A path with lesser weight (shorter path), to ux is found  
              if alt < distance[ux]:                 
                  distance[ux] = alt            // updating the distance of ux   
  
      return dist[]  
  end Method  
