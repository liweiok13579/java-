# java-
get 查询然后return 出去
set  类似于attr  增加一个值
public 创建java后缀的时候选择public选择公众包（可以被别的调用），package 私有包裹（类似于闭包）
右键点击source，然后选择Generate Getters and setters to create；可以快捷出来 name和password的get和set方式。
定义方法：
       public公开的
       static静态（没有数据）
       void（没有返回值）
       public static void main(String[] args) {
          Users user = new Users();
          user.setName("伟伟");
          user.setPassword("weiwei");
          test1(user);
        }
java后缀的文件首字母大写；
equals（name）判断地址，也可以判断值相等不相等
控制台输出 System.out.println("登录成功");
      package lw;
        
      import pojo.User;

      public class Login {
        public static void main(String[] aa){
          User a1= new User();
          a1.setName("admin");
          a1.setPassword("123456789");
          bb(a1);
        }
        public static void bb(User user){
          String name = user.getName();
          String ps = user.getPassword();
          if("admin".equals(name)&&"123456789".equals(ps)){
            System.out.println("登录成功");
          }else{
            System.out.println("登录失败");
          }
        }
      }
