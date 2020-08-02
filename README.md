
### 定义5个类和面向对象的东西

class People:  #定义一个人类
    #定义属性
    eye = "black"
    skin = "yellow"
    #定义方法
    def eat(self):
        print(f"会用筷子吃饭")
    def say(self):
        print("会说中文")
xm = People()  #类的实例化
print(f"小明的眼睛是：{xm.eye}，皮肤是{xm.skin}")  #输出实例化属性
xm.eat()   #调用方法，输出eat方法
xm.say()   #调用方法，输出say方法


class Fan(): #定义风扇类
    # 定义属性
    fender = 3
    case = "金属"
    # 定义方法
    def run(self):
        print("风扇的能量是靠充电的")
    def wind(self):
        print("能吹凉快的风，使人感到舒适")
MD=Fan()  #类的实例化
print(f"风扇由{MD.fender}片叶子组成，外壳是{MD.case}做的")  #输出实例化属性
MD.run()   #调用方法，输出run方法
MD.wind()  #调用方法，输出wind方法


class Cat:  #定义猫的类
    # 定义属性
    name = "jimi"
    hair = "white"
    leg = 4
    # 定义方法
    def say(self):
        print("会喵喵叫")
    def eat(self):
        print("爱吃鱼")
    def jump(self):
        print("会跳")
cat=Cat()   #类的实例化
print(f"猫的名字叫{cat.name},他有{cat.leg}条腿，毛发是{cat.hair}")   #输出实例化属性
cat.say()   #调用方法，输出say方法
cat.eat()   #调用方法，输出eat方法
cat.jump()   #调用方法，输出jump方法


















