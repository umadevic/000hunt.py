n,u,m=map(int,input().split())
lis=list(map(int,input().split()))
h=list(combinations(lis,u))
for i in range(0,len(h)):
    y=list(h[i])
    w = 0
    for j in range(0,u):
        w=w+y[j]
    if w==m:
        print("YES")
        sys.exit()
print("NO") 
