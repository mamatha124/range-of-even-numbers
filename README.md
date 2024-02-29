# range-of-even-numbers in python
# range or mean of even numbers
# Approaach-1
n=int(input())
a=list(map(int,input().split()))
es=0
c=0
for i in range(n):
  if a[i]%2==0 and a[i]>es:
    es=es+a[i]
    c=c+1
print(es//c)
 
# approach-2
n=int(input())
a=list(map(int,input().split()))
es=0
c=0
for i in a:
  if i%2==0 and i>es:
    es= es + i
    c=c+1
print(es//c)

# approach-3
n=int(input())
a=list(map(int,input().split()))
e=[]
for i in range(n):
  if a[i]%2==0:
    e.append(a[i])
print(sum(e)//len(e))
