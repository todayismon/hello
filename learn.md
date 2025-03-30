<details>

<summary>Tips </summary>
qwerttyyuuiiiooooooooooooppppppppp
iiiiii

ioioioooooo

</details>

```ruby
   puts "Hello World"
```



> [!TIP]
> this is a tip.



```python
#1010 任意大整数
def dfs(x):
	s= ()
	for i in reversed(range(x.bit_length())):
		if (x>>i)&1:
			if i>1:
				s+= '2('+dfs(i)+')',
			elif i==1:
				s+= '2',
			else:
				s+= '2(0)',
	return '+'.join(s)
print(dfs(int(input())))


#1116
import sys
n,*a= map(int, sys.stdin.read().split())
c= 0
for i in range(n):
	for j in range(i):
		if a[j]>a[i]:
			c+= 1
print(c)


#5143
import sys,math
n,*a= map(int, sys.stdin.read().split())
a= sorted([(a[i+2],a[i+1],a[i]) for i in range(0,3*n,3)])
q=0
for i in range(n-1):
	z0,y0,x0= a[i]
	z1,y1,x1= a[i+1]
	q+= math.sqrt((z1-z0)**2+(y1-y0)**2+(x1-x0)**2)
print(round(q,3))


#1068
import sys,math,bisect
n,m,*a= map(int, sys.stdin.read().split())
a= sorted([ (-a[i+1],a[i]) for i in range(0,2*n,2) ])
v= a[math.floor(1.5*m)-1][0]
i= bisect.bisect_right(a, v, key=lambda c:c[0])
print(-v,i)
for x,y in a[:i]:
	print(y,-x)
```