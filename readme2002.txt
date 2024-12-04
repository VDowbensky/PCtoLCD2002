The first beta version was released at midnight on May 1. Function introduction: 
1. Generate font data of mixed Chinese, English and digital strings. 
2. You can select the font and size, and adjust the length and width of the text independently to generate characters of any shape. 
3. Various rotation and flip text functions 
4. Adjust the output dot matrix size and the position of the characters in the dot matrix at will. 
5. The font data output can be customized in various formats. The system presets two formats, C language and assembly language, and you can define a new data output format by yourself; the number of output data per line is adjustable. 6. Support four modes of modulo: row by row (that is, taking points row by row horizontally), column by column (taking points column by column vertically), row and column (first
take the 8 points of the first row horizontally as the first byte, then take the 8 points of the second row vertically as the second byte...),
column and row (first take the first 8 points of the first column vertically as the first byte, then take the first 8 points of the second column horizontally as the second
byte...)
7. Support Yin code (bright spot is 1), Yang code (bright spot is 0) modulo
8. Support vertical (the first bit is low) (, reverse the first bit is high) modulo
9. The output number system can be selected as hexadecimal or decimal
10. Index files can be generated to quickly retrieve the required Chinese characters in the large number of generated character libraries
11. Dynamic LCD panel simulation, the pixel size and color of the simulation panel can be adjusted
12. In graphic mode, you can draw with the mouse at will, the left key draws, and the right key erases.
12. The functions in character mode such as rotation, flipping, and translation can also be used to process BMP images. The version is pctolcd1.94

5月1日晚上发布第二测试版
  更新如下:
  1.增加锁定点阵大小功能，例如可锁定24X24点阵大小，然后调节独立调节字点阵的大小
  2.增加热键功能，可用光标配合Ctrl,Shift对文字大小和位置修改
  3.增加精简输出格式选项
  4.把文字输入框换成了文字输入组合框，这样就可以保存历史纪录。
  5.输出数据会自动清除以前的数据
  6.可隐藏自定义格式，简化操作
  7.一些小的BUG修正。
 版本为pctolcd2.03

5月3日凌晨发布第三测试版
 更新如下:
 1.增加了一些小东西，例如演示动画一类的，我懒的一一写了
 2.改掉一些可恶的小BUG，例如点阵输入框的自动完成。
 3.增加大量文字处理和导入TXT文本文件功能，并且可以去除文本中的空白和重复字符，
   可以对文本进行排序，适合于生成小字库。我这里测试是3万多字的TXT文件在2分钟内转成16X16点阵的字库文件。

版本号为pctolcd2.53

由于本软件侧重于对字符的处理，所以在图象方面功能较弱，请见晾。



5月8日发布正式版

   正式版已经开始朝着液晶字库生成软件的方向进化了,我在后来的更新中把主要精力也放
在这部分,由于我目前还没有发现有同类的软件具备这个功能,也无法得到任何的参考,只能
自己摸索前进,所以如果还有不方便的地方请大家多提意见.
具体更新如下:
 1.重写大部分的内核代码以配合汉字库生成的功能,目前这个内核已经进行了反复的测试,
相信稳定性和速度较前一版本有了巨大的提高.
 2.去掉那个比较愚蠢的热键区了,因为用处不大
 3.增加汉字库生成功能,这是最重要的改进之处,下文将详细介绍.
 4.修正许多小BUG,使软件更加成熟些.

  
5月12日发布完美版

  这次发布的PCtoLCD2002完美版与前一版本相比没有增加太多的功能，因为我觉得现有的这些功能已经足够用于生成各种字模的需要了，所以完美版的主要工作是反复测试，精心去除各种BUG，以及调节一些细微之处，目的当然就是追求完美！不过世上不会有真正完美的东西，这个软件也不例外，而且这个软件从头至尾全部是我一个人编写完成，精力有限，难免会顾此失彼，如果大家发现了这个版本中存在的BUG，请及时告诉我。
    更新说明：
   1。界面采用新的字体，不会再有那种难看的黑色粗体字，比以前的要漂亮多了。
   2。加入全面的提示帮助，尽量减少普通用户的各种疑惑。
   3。修正生成文件的扩展名的一些BUG，不会总是加上FON的扩展名了。
   4。修正生成字模数据的一些格式BUG，现在生成的C51格式字模数据基本上可以直接粘贴到源程序中使用而不需要修改了
   5。加入新的字模数据格式调整项，允许用户更自由的定制自己需要的数据格式
   6。最重要的更新：全面支持保存当前设置功能，用户设置的字模格式，主窗口状态和字库生成窗口选项信息均可保存，下一次打开窗口时不用重新设置。
   7。修正了新建图象时会自动跳到图形模式的BUG
   8。增加输出紧凑格式数据选项，可以生成不包含空白行的字模数据。
   9。完善了每行数据显示个数的功能，可以任意设置每行显示的数据个数，并同时可以设置每行索引数据显示个数。
   10。修正了取模说明的一些错误，并改动了格式。
   11。现在当用户选择10进制输出时，会自动去掉生成字模数据前的“0x",或后面的“H”，选择16进制时则会自动加上。
   12。对各个窗体重新设计以全面适应最大化的需要，如果您觉得当前窗口不够大，可以最大化使用。
   13。增加生成英文点阵字库功能，可自动生成ASCII码从0-127的任意点阵字库，使用方法同生成国标点阵字库功能。
   14。再次优化代码，去掉各种调试信息，使程序速度再快一些。
   15。还有许多细微的调整我记不清了……

需要注意的地方：
  在测试的过程中我发现了一个问题：在WIN98或WINME下当用户直接生成特大点阵的字模时（例如320*320，1024*768的汉字字模），此时由于数据量非常庞大，而WIN98/WINME会有64K的数据容量限制，所以在主窗口中是无法得到全部的字模数据的，这时您需要使用字库生成功能，通过形成一个数据文件才能得到完整的字模数据。



我认为到现在这个软件功能已经很完善了，但可能使用上有点不方便，如果你有什么不明白
的地方，可以发帖子或发MAIL询问



