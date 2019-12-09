一、实验目的：
分析学生选课系统
使用GUI窗体及其组件设计窗体界面
完成学生选课过程业务逻辑编程
基于文件保存并读取数据
处理异常

二、要求
1、	设计GUI窗体，支持学生注册、课程新加、学生选课、学生退课、打印学生选课列表等操作。
2、	基于事件模型对业务逻辑编程，实现在界面上支持上述操作。
3、	针对操作过程中可能会出现的各种异常，做异常处理。
4、	基于输入/输出编程，支持学生、课程、教师等数据的读写操作。

三、流程图

![](https://github.com/LIUCHANGYOU6/liu/blob/master/1.png)

四、核心代码
1.
   FileWriter writer;
	        try {
	            writer = new FileWriter("C:\\Users\\46975\\Desktop\\java实验\\exp5\\T.txt",true);
	            writer.append(s6); 
	            writer.flush();
	            writer.close();
	        } catch (IOException e1) {
	            e1.printStackTrace();
	        }
          
2.
      try {
		  BufferedReader br = new BufferedReader(new FileReader("C:\\Users\\46975\\Desktop\\java实验\\exp5\\T.txt"));
		    String Student_num = br.readLine();
		    br.close();
		    writer = new FileWriter("C:\\Users\\46975\\Desktop\\java实验\\exp5" + Student_num +".txt",true);		                    writer.append(chosen); 
		    writer.close();
           } catch (IOException e1) {
		            e1.printStackTrace();
		        }
			
五、运行结果
![](https://github.com/LIUCHANGYOU6/liu/blob/master/3.png)
![](https://github.com/LIUCHANGYOU6/liu/blob/master/2.png)
