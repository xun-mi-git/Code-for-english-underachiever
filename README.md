# Code-for-english-underachiever（英语差生也能敲代码）
此工具是帮助英语单词量少的可怜的（说的就是本人自己了）的人背单词。
## 项目使用技术
1. Python作为基础开发语言
2. 单词以TXT文件形式存储（原本考虑过数据库，但是因为数据量较小，而且成本较高，所以决定使用简单粗暴的.TXT进行存储）
3. 存储以*单词-使用含义（在代码中的含义）-实际含义*

## 项目1.0版本计划
1. 随机抽取单词，输出其汉意，并让使用者输入对应的单词，判断对错，并在错误三次后提示。
2. 使用者可以对TXT文件中的单词以及对应的含义进行增删改查。
3. 实现GUI界面
4. 对每个单词输入对错次数进行统计
5. 接入翻译接口，可以对单词进行在线翻译以及朗读
6. 尝试根据对错单词输入的对错情况对单词输出概率进行影响，让输入错的的单词出现的概率大幅增加，减少输入正确的单词的出现概率
7. 将存入单词进行日常使用度分类初步计划分为三类，日常操作会使用的为第一类，术语形为第二类，有关联性的单词为第三类
## 使用逻辑
1. 输入正确提示正确，并进行下一个单词输出
2. 默认输入错误三次提示正确答案，此处值可以修改。
3. 如果输入为空，则表示不知道输出正确答案
4. 空格表示跳过此问直接输出下一问题，输入OK表示已经完全记住此单词之后如果碰到则自动跳过