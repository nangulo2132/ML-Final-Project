# ML-Final-Project
New York City has one of the most extensive public transit systems in the world, and yet millions of
residents live beyond walking distance of any subway station. The MTA’s proposed Interborough Express
(IBX) is itself an acknowledgement that the existing network falls short for cross-borough commuting. The IBX, which the MTA claims will benefit traditionally underserved communities, would run along the southern part of Brooklyn and Queens, connecting neighborhoods that currently have no direct transit link (MTA, 2022).

This project investigates whether a GraphSAGE encoder trained on origin-destination (OD) commuter flows and subway stop accessibility can identify underserved transit corridors better than a simple demand-rank heuristic. We define an “underserved” corridor as an OD pair where demand meets or exceeds the median (6 workers per pair) and neither endpoint has a subway stop within 800 meters, roughly a half-mile walk. The demand-rank heuristic knows only how busy a corridor is, while the GNN knows the whole neighborhood context.

Graph neural networks (GNNs) are a class of deep learning model that analyzes data in the form of a graph, or network of interconnected nodes and edges. GNNs specialize in non-Euclidean data with irregular structural designs. Transit systems are inherently graph-shaped, with many nodes and edges representing how people move around a city, making GNNs a natural fit for this problem.
