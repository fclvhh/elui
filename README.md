"# elui" 
 ## js实现的思路的不同

原生的js: 有好用的的forEach()
但是jQuery 全是jQuery 对象 , 好像不能用forEach()

原生的思路 : 
- 父亲获取所有的孩子 . 一起"熄灭自己"
- 父亲的所有孩子依次遍历 . 添加事件
  - 这是很麻烦的
  - jQuery采用了 事件代理
    - e.target / e.currentTaeget 获取触发点
    - 这样一次绑定就好了
    - 新的问题 ; 触发点 的 index 是未知 代求的
  - 相对来说 , 这点 forEach( ) 就好很多了
jQuery的思路: 
- 事件代理
- sibling() 同辈移除

