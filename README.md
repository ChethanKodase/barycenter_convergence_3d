# Barycenter convergence on 3d point clouds

Different point cloud with points sampleed from different three dimensional geometrical objects have different topological features. Persistence homology is one
of the methods to capture topological features of the maniold from which the points are being sampled. If there are too many points in the dataset, calculation of
persistence homology becomes very expensive. It is easier to calculate persistence homology for lesser number of points with same manifold feutures.
Barycenter sampling methods enable us to sample the points from the dataset, at the same time preserving the global topolgy of the original manifold within the sampled
points.

## Steps in barycenter sampling method for 3d point clouds

Step 1: Consider a 3d point cloud and a random initial point.

Step 2: Find out n nearest neighbours of the initial point and then find the centroid of the sampled neighbours.

Step 3: Again find n neighbours to the centroid and continue the same until there is convergence of centroid, i.e, when same neighbours are sampled in a successive step.

Step 4: Once the centroid converges, eliminate all the points that came along the way and the centroid of convergence is sampled as the barycenter.

Step 5: Again start from step 1
