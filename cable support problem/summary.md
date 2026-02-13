
<img width="1699" height="1006" alt="image" src="https://github.com/user-attachments/assets/bd1fabc7-1ecf-4ecc-804a-046a541debfd" />


# Cost Functions:

```math

c(e) = dist(e)


```

```math
t(e, \pi) = dist(e)*6
```

# Algorithm Analysis

| Cost Framework | Algorithm Name | Description | Total Cable Length | Total Tray Length *6 | Total Cost | <div style="width:400px">Visualization</div> |
|---|---|---|---|---|---|---|
|  	Tray cost = (length meter of edge used in any path * 6), 	Cable cost = (total length of all paths in meters)  | Dijkstra Shortest Path |  Shortest path, minimizing total cable length, ignoring tray costs.  | 95.6 | 344.61 | 440.21 |  <img src="animation_gifs\Sample Project with Dijkstra Shortest Path.gif" style="width:400px" align="left"/>|
|  	Tray cost = (length meter of edge used in any path * 6), 	Cable cost = (total length of all paths in meters)  | Prioritized Dijkstra Shortest Path |  Sequentially running Dijkstra, laying down tray at each step, minimizing total cost tray costs.  | 153.38 | 299.54 | 452.92 |  <img src="animation_gifs\Sample Project with Prioritized Dijkstra Shortest Path.gif" style="width:400px" align="left"/>|
|  	Tray cost = (length meter of edge used in any path * 6), 	Cable cost = (total length of all paths in meters)  | Prioritized Dijkstra Shortest Path with 5 Restarts |  Sequentially running Dijkstra, laying down tray at each step, minimizing total cost tray costs. Permutes the order of cables to attempt to find lower cost solutions. Restarts = 5  | 167.83 | 278.52 | 446.35 |  <img src="animation_gifs\Sample Project with Prioritized Dijkstra Shortest Path with 5 Restarts.gif" style="width:400px" align="left"/>|

