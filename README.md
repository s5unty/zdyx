# 哲豆音形输入法(弄堂版)

## 哲豆音形原版介绍

- [哲豆音形官网][1]
- [哲豆音形RIME版][2]
- 哲豆音形键位图
<details><summary>显示键位图</summary>

![](https://du1ab.one/images/2022/zdyx_keyboard.jpg)
</details>

## 与原版的主要差异

1. 字典与词典分离，词典不再依赖硬性编码
2. 单字拥有了权重，[借鉴自][3] Rime 五笔字典
3. 移除了U键(飞Q)和I键(飞Z)的声母飞键功能
4. 重新定义了词组的编码格式，最长6码
5. 拼音反查键，由 \` 改为 `i`

    ![](https://du1ab.one/images/2022/fancha.gif)

## 弄堂版的特点说明

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
  * `jlstjc` 计 `jlff` 算 `stoa` 机 `jcww`
  * `mbzfjb` 民 `mbcc` 政 `zftk` 局 `jbii`

  同时，也引入了 2+2 大写模式，用于后两个字的简拼。便于输入一些音译词或是人名。例如：
  * `ldSJ` 洛 `ldwi` 杉/衫 `S` 矶 `J`
  * `dfJH` 丁 `dfff` 俊 `J` 晖/辉 `H`

* 四字以上，由定长4码，改为了定长6码——头两字前2后1，尾两字前2后1，例如：
  * `baylts` 布 `baoi` 宜 `ynod` 诺斯艾利 `ltuu` 斯 `sfqi`
  * `zoyslt` 中 `zoii` 央 `yokk` 电视 `sloc` 台 `tlii`

  同时，也引入了 3+2 大写模式，用于后两个字的简拼。便于输入一些音译词或是人名。例如：
  * `jnlNY` 加 `jzii` 利 `ltuu` 福尼 `N` 亚 `Y` —— N键(飞Z)的笔形飞键功能，仍然有效
  * `lonED` 罗 `lowk` 纳 `nyok` 尔 `E` 多 `D`

  ![](https://du1ab.one/images/2022/34zici.gif)

* 整句的连续输入，前提是字/词无重码(位于首选)

  ![](https://du1ab.one/images/2022/sentence.gif)

* 支持 3 字以内词组的自动造词，常用于口头语，或人名地名
* 支持 4 码以上字词的动态调频，单字简码(1/2/3)不受影响

[1]: http://zzdzzd.ysepan.com/
[2]: https://github.com/whjiang/zzdyx_rime
[3]: https://gist.github.com/s5unty/08c3a6d7429c65a37b4b4aaaf3f9bed5

