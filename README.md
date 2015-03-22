## Sample run:
## > x = rbind(c(1, -2), c(-2, 1))
## > mc = makeCacheMatrix(x)
## > mc$get()
##       [,1] [,2]
##  [1,]    1   -2
##  [2,]   -2    1

## No cache in the first run
## > cacheSolve(mc)
##            [,1]       [,2]
## [1,] -0.3333333 -0.6666667
## [2,] -0.6666667 -0.3333333

## Retrieving from the cache in the second run
## > cacheSolve(mc)
## getting cached data.
##            [,1]       [,2]
## [1,] -0.3333333 -0.6666667
## [2,] -0.6666667 -0.3333333
