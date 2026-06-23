# MINIMUM SPANNING TREE- PRIMS ALGORITHM 
# SAMPLE INPUT 
#0 2 3
#2 0 1
#3 1 0
#SAMPLE OUTPUT 
# TOTAL WEIGHT =3
# Prim's Algorithm 

n = int(input("Enter number of vertices: "))

print("Enter the adjacency matrix:")
graph = []

for i in range(n):
    row = list(map(int, input().split()))
    graph.append(row)

selected = [False] * n
selected[0] = True

edge_count = 0
total_cost = 0

print("\nEdges in MST:")

while edge_count < n - 1:
    minimum = float('inf')
    x = 0
    y = 0

    for i in range(n):
        if selected[i]:
            for j in range(n):
                if not selected[j] and graph[i][j] != 0:
                    if graph[i][j] < minimum:
                        minimum = graph[i][j]
                        x = i
                        y = j

    print(f"{x} - {y} : {graph[x][y]}")
    total_cost += graph[x][y]
    selected[y] = True
    edge_count += 1

print("\nMinimum Cost =", total_cost)

