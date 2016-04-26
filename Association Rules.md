#####参见网站：
- http://www.17bigdata.com/%E5%85%B3%E8%81%94%E8%A7%84%E5%88%99%E7%9A%84%E5%B8%B8%E7%94%A8%E7%AE%97%E6%B3%95.html
- http://cs.sjtu.edu.cn/~yshen/courses/BigData 课程网站
关联规则（Association Rules）是一种广泛使用的模式识别方法
目的是找到事物之间的联系

#####判定事物关联的标准
- Support ： *I*项的support意味着 含有*I*的basket 个数

  Support threshold：给出一个support threshold 那么比这个值高的support I项就叫做常见项

- ![](http://latex.codecogs.com/gif.latex?{i_1,i_2,...,i_k} \\to j) 意味着
  如果一个basket里面有 i1，i2，...,ik 那么他**很有可能**也有j
  
- Confidence ：
  ![](http://latex.codecogs.com/gif.latex?conf(I \\to j) = \\frac{support(I \\cup j)}{support(I)})
- Interest :
   ![](http://latex.codecogs.com/gif.latex?conf(I \\to j) = \\frac{support(I \\cup j)}{support(I)}- Pr[j])
   
   注意 Interest 相比于 Confidence 惩罚了j的频率，防止有些事物出现的事物太频繁，而形成了几乎所有项集都和它有关的局面
  
  
  
