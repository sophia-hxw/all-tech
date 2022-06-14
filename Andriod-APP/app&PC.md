## 接口设计
- 数据传输方式，XML和json
- 数据类型
    - app端涉及加、减、乘、除和比较大小，用double型；   
    - 布尔型的也用double替代；
    - 其他统一用字符串型；
- app从服务器读取数据为空时，返回相应数据类型的"空"，而不是null
- 数据交互时，带版本号，应对接口代码改变；
- app显示的图片需要处理时，将处理过程放在服务器端；
- 传输数据用http连接
- 向app返回数组数据应该支持分页操作；
- 可能会变动的功能逻辑，尽量放在服务器端实现；
- app要注意处理crash问题，尤其涉及数据解析问题；
- 服务器设计端口时考虑app重复提交数据的情况；


## 安全方案

### http方法使用
- get和post区别
    get的参数在url里，post参数在body里，从安全上考虑，尽量用post；

