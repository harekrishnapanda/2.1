# 2.1.1
def addn(x,y):
    return(x*y)

def myreduce(funcy,lsst):
    result = 0
    for z in lsst:
        if z == lst[0]:
            result = funcy(lsst[0],lsst[1])
        elif z == lsst[1]:
            result = result
        else:
            result = funcy(result,z)
    print(result)
    
lst= [1,2,3,4]
myreduce(addn,lst)


# 2.1.2
def myfilter(funcy,lsst):
    templist=list()
    
    for x in lsst:
        if funcy(x)==True:
            templist.append(x)
    print(templist)
    
def even_check(num):
    if num%2 == 0:
        return True
    
lst =range(20)    
myfilter(even_check,lst)
