sugar=50
teapowder=200
oil=150
salt=20
oats=270
cname=input('enter customer name:')
cpho=int(input('enter customer phone:'))
sugarkgs=int(input('enter sugar kgs:'))
teapowderkgs=int(input ('enter teapowder kgs:'))
oilkgs=int(input ('enter oil kgs:'))
saltkgs=int(input('enter salt kgs:'))
oatskgs=int (input ('enter oats kgs:'))
bill=(sugar*sugarkgs)+(teapowder*teapowderkgs)+(oil*oilkgs)+(salt*saltkgs)+(oats*oatskgs) 
if bill>=5000:
    disc=bill*10/100
    tax=0
elif bill>=3000:
    disc=bill*8/100
    tax=bill*10/100
elif bill>=2000:
    disc=bill*5/100
    tax=bill*18/100
elif bill>=1000:
    disc=bill*3/100
    tax=bill*18/100
else:
    print('no shopping')
mainbill=bill-disc+tax
print ('bill amount:',mainbill)
