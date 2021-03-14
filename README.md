# graph-encyptionimport matplotlib.pyplot as plt


x=int(input('enter x '))
x2=int(input('enter x2 '))
x3=int(input('enter x3 '))
x4=int(input('enter x4 '))



#plotting a graph in respect to x,y=x**2 
function ={'hello':[x,x**2],'how':[x2,x2**2],'are':[x3,x3**2],'you':[x4,x4**2]}
function2={'hello':x,'how':x2,'are':x3,'you':x4}
function3={'hello':x*2,'how':x2*2,'are':x3*2,'you':x4*2}



#plotting the number
x,y=function['hello']
x2,y2=function['how']
x3,y3=function['are']
x4,y4=function['you']

#plotting he function u choose
z=[x,x2,x3,x4]
u=[y,y2,y3,y4]

print( z,u )

#plotting the derivative of the function u choose
X=int(input('enter X '))
X2=int(input('enter X2 '))
X3=int(input('enter X3 '))
X4=int(input('enter X4 '))

yderv=2*X
yderv2=2*X2
yderv3=2*X3
yderv4=2*X4


dx=[X,X2,X3,X4]
dy=[yderv,yderv2, yderv3, yderv4 ]


while X!=x:
    X=int(input('enter X to compeare the gtraph to the dirivat'))
    print("x not = to X "  )
    if X>x:
         print("sorry X greater than x , guess again")
    elif X<x:
           print ('sorr X less than x,guess again' )     

    if X==x:
           print('x=X')
    decription={v:u for u,v in function2.items() }
    print (decription)
    


"""while X2!=x2:
    X2=int(input('enter X to compeare the gtraph to the dirivat'))
    print("x not = to X "  )
    if X2>x2:
         print("sorry X greater than x , guess again")
    elif X2<x2:
           print ('sorr X less than x,guess again' )     

print('x2=X2')"""

"""while X3!=x3:
    X3=int(input('enter X to compeare the gtraph to the dirivat'))
    print("x not = to X "  )
    if X3>x3:
         print("sorry X greater than x , guess again")
    elif X3<x3:
           print ('sorr X less than x,guess again' )     

print('x=X')
X=x"""

decription={v:u for u,v in function2.items() }
print (decription)
print(y2)
print(yderv2)



"""if yderv==y2 :
    
    print('yderv1 =  y2')
if yderv2==y2:
    print('yderv2 =  y2')
if yderv3==y2:
    print ('yderv3 = y2')
if yderv4==y2:
    print('yderv is = to y2')"""


decription2={v:u for u,v in function3.items() }

plt.plot(dx,dy)
plt.plot(z,u)
plt.xlabel('x')
plt.ylabel('y')
plt.title('encripted graph')
plt.show()


      
