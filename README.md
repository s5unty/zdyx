# 哲豆音形输入法(弄堂版)

## 哲豆音形原版介绍

- [哲豆音形官网][1]
- [哲豆音形RIME版][2]
- 哲豆音形键位图
<details>
  <summary>显示键位图</summary>

  ![](http://ys-f.ysepan.com/58342039/115098388/lMOeLjk4H546F27KHMJ31b/%E5%93%B2%E8%B1%86%E9%9F%B3%E5%BD%A2%E5%A4%A7%E5%9C%86%E6%BB%A1%E7%89%88%E9%94%AE%E7%9B%98%E5%9B%BE.jpg)

</details>

## 与原版的主要差异

1. 字典与词典分离，词典不再依赖硬性编码
2. 单字拥有了权重，[借鉴自][3] Rime 五笔字典
3. 移除了U键(飞Q)和I键(飞Z)的声母飞键功能
4. 重新定义了词组的编码格式，最长6码

## 弄堂版的编码格式

* 单字，和原版相同，包括简码(1/2/3)和全码(4)

  ![](https://du1ab.one/images/2022/1jian.gif)

* 二字词，由定长4码，改为了最长6码——每个字取前3码

  拥有2级简码的字，在组二字词时，该字可以省略第3码。  
  示例中的「南/上/海」，都有对应的2简，在组词时，该字只需2码。  
  如果打满6码，则不用空格确认，被随后的输入自动顶上屏。  

  ![](https://du1ab.one/images/2022/2zici.gif)

  「京」字没有2简，「南京」至少需要打5码—— `nfjhi`。  
  经过两次输入确认、完成了自动组词之后，只需要打4码 `nfjh`。

* 三字词，由定长4码，改为了定长6码——每个字取前2码，例如：

  ** `jlstjc` 计 **jl**ff 算 **st**oa 机 **jc**ww
  ** `mbzfjb` 民 **mb**cc 政 **zf**tk 局 **jb**ii

  同时，也引入了 2+2 大写模式，用于后两个字的简拼。使一些音译词易于输入。例如：

  ** `ldSJ` 洛 **ld**wi 杉/衫 **S** 矶 **J**

* 四字以上，由定长4码，改为了定长6码——头两字前2后1，尾两字前2后1，例如：

  ** `baylts` 布 **ba**oi 宜 **y**nod 诺斯艾利 **lt**uu 斯 **s**fqi
  ** `zoyslt` 中 **zo**ii 央 **y**okk 电视 **sl**oc 台 **t**lii

  同时，也引入了 3+2 大写模式，用于后两个字的简拼。使一些音译词易于输入。例如：

  ** `lonNA` 罗 **lo**wk 纳 **n**yok 尔迪尼 **N** 奥 **A**

  ![](https://du1ab.one/images/2022/34zici.gif)

[1]: http://zzdzzd.ysepan.com/
[2]: https://github.com/whjiang/zzdyx_rime
[3]: https://gist.github.com/s5unty/08c3a6d7429c65a37b4b4aaaf3f9bed5

