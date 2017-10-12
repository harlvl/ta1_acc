# ta1_acc

## Para probar las soluciones:

### 1) DFS

```
python pacman.py -l tinyMaze -p SearchAgent
```
```
python pacman.py -l mediumMaze -p SearchAgent   --frameTime 0
```
```
python pacman.py -l bigMaze -z .5 -p SearchAgent -z .5 --frameTime 0
```

### 2) BFS

```
python pacman.py -l tinyMaze -p SearchAgent -a fn=dfs
```
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs --frameTime 0
```
```
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs -z .5 --frameTime 0
```

### 3) A*

```
python2 pacman.py -l mediumCorners -p SearchAgent -a fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic
```

### 4) Distance Euclidian

```
python pacman.py -l mediumCorners -p SearchAgent -a fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic -z 0.5
```
```
python pacman.py -l bigCorners -p SearchAgent -a fn=aStarSearch,prob=CornersProblem,heuristic=cornersHeuristic -z 0.5
