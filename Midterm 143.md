# Midterm 143

* 如果要修改一个list里面的东西，要用iterator而不是for-each loop 会出现并行修改的exception

### recursion tracing

- 列表：每次有一个数值更新都要在草稿本上更新
- recursive的method 和 print的顺序 print在后面的话就先在后面写没更新的值
- 如果实在算不明白的话把每个recursion的数字带进去 然后把method写下来 写到最后就是
  - method（x）+method（x+1）之类的，然后每个method再去解顺序就不会错
  - 见下图
- 除非规律极其明显 否则不建议跳步

### llinked list node manipulation

- 画图！画图！！画图！！！
- 每次更新之后都要看两条node分别的变化是什么，再考虑下一步怎么写
- 如果写熟练了，画箭头的时候也要注意标上步数
- 先移后面的，再移前面的
- 如果一条node在最后是空的，最后一句一定要加xx.next = null; 这样以防万一
- 分清谁指向谁，不要写反
- a指向b，a多写一个next

### Recursive Programming

- 弄清楚 base case和特殊情况
- 写一个多加一个参数的helper method
- 复习substring
- string题一般就是多加一个charAt哪个index的参数，然后每个index call的时候加1
- 除了base case 和特殊情况 return都要call自己 如果没call那大概是错了

### Collection Programming

- 不可以直接写Map xx = new Map, order是TreeMap， 别的是hashMap
- 