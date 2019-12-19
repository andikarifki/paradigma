def dist2D( p ):
    return (p[0]**2 + p[1]**2)**0.5
pts = [ (4.5, 3), (2.1,-1), (6.8,-3), (1.4, 2.9) ]
print(max( map(dist2D,pts) ))