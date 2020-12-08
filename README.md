menuList = []

systemMenu = {"ข้าวหมกไก่":45,"ข้าวมันไก่":40,"ข้าวมันไก้่ผสม":50,"ข้าวมันไก่พิเศษ":45 }


def showBill():

    totalPrice = 0
    
    textShowmenu = "My Food"
    
    print(textShowmenu.center(21,"-"))
    
    for number in range(len(menuList)):
    
        print(menuList[number][0],menuList[number][1]"THB")
        
        totalPrice += int(menuList[number][1])
        
    print("Total Price(THB) :",totalPrice)
    

while True:

    menuName = input("Plese Enter Menu :")
    
    if(menuName.lower() == "exit"):
    
        break
        
    else:
    
        menuList.append([menuName,systemMenu[menuName]])
        

showBill()
