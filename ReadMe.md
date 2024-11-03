# 1.创建RTSManager蓝图框架文件

![image-20241103211639466](./ReadMe.assets/image-20241103211639466.png)

![image-20241103211653012](./ReadMe.assets/image-20241103211653012.png)

2.在PlayerController中对相关快捷键进行添加（使用增强输入文件）

![image-20241103211808178](./ReadMe.assets/image-20241103211808178.png)

![image-20241103211832167](./ReadMe.assets/image-20241103211832167.png)

# 3.HUD中设置框选的类型和颜色

![image-20241103212051546](./ReadMe.assets/image-20241103212051546.png)

注意：DrawColor的Alpha值不能为0，否则无法看到框选形状

# 4.可以框选的单位必须添加组件SelectedActor

![image-20241103212204545](./ReadMe.assets/image-20241103212204545.png)

该组件有三个触发委托，符合条件进行触发

![image-20241103212342793](./ReadMe.assets/image-20241103212342793.png)

# 5.进行阵列移动的单位必须添加组件AdvancedBehavior

![image-20241103212252727](./ReadMe.assets/image-20241103212252727.png)

该组件有两个触发委托，符合条件进行触发

![image-20241103212404810](./ReadMe.assets/image-20241103212404810.png)

# 6.建造判断请继承JudgmentBuild类

![image-20241103212459920](./ReadMe.assets/image-20241103212459920.png)

该类中判断的核心通过下面函数

![image-20241103212625104](./ReadMe.assets/image-20241103212625104.png)

return Value的值如果为true，说明当前可以建造，返回可建造的坐标，以及当前的旋转值



# 注：更多函数可以在对应的类中右键搜索RTSManager

![image-20241103212901631](./ReadMe.assets/image-20241103212901631.png)![image-20241103212926284](./ReadMe.assets/image-20241103212926284.png)![image-20241103213005584](./ReadMe.assets/image-20241103213005584.png)

或参考项目示例