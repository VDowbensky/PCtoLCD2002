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

5��1�����Ϸ����ڶ����԰�
  ��������:
  1.�������������С���ܣ����������24X24�����С��Ȼ����ڶ��������ֵ���Ĵ�С
  2.�����ȼ����ܣ����ù�����Ctrl,Shift�����ִ�С��λ���޸�
  3.���Ӿ��������ʽѡ��
  4.����������򻻳�������������Ͽ������Ϳ��Ա�����ʷ��¼��
  5.������ݻ��Զ������ǰ������
  6.�������Զ����ʽ���򻯲���
  7.һЩС��BUG������
 �汾Ϊpctolcd2.03

5��3���賿�����������԰�
 ��������:
 1.������һЩС������������ʾ����һ��ģ�������һһд��
 2.�ĵ�һЩ�ɶ��СBUG����������������Զ���ɡ�
 3.���Ӵ������ִ���͵���TXT�ı��ļ����ܣ����ҿ���ȥ���ı��еĿհ׺��ظ��ַ���
   ���Զ��ı����������ʺ�������С�ֿ⡣�����������3����ֵ�TXT�ļ���2������ת��16X16������ֿ��ļ���

�汾��Ϊpctolcd2.53

���ڱ���������ڶ��ַ��Ĵ���������ͼ���湦�ܽ������������



5��8�շ�����ʽ��

   ��ʽ���Ѿ���ʼ����Һ���ֿ���������ķ��������,���ں����ĸ����а���Ҫ����Ҳ��
���ⲿ��,������Ŀǰ��û�з�����ͬ�������߱��������,Ҳ�޷��õ��κεĲο�,ֻ��
�Լ�����ǰ��,����������в�����ĵط����Ҷ������.
�����������:
 1.��д�󲿷ֵ��ں˴�������Ϻ��ֿ����ɵĹ���,Ŀǰ����ں��Ѿ������˷����Ĳ���,
�����ȶ��Ժ��ٶȽ�ǰһ�汾���˾޴�����.
 2.ȥ���Ǹ��Ƚ��޴����ȼ�����,��Ϊ�ô�����
 3.���Ӻ��ֿ����ɹ���,��������Ҫ�ĸĽ�֮��,���Ľ���ϸ����.
 4.�������СBUG,ʹ������ӳ���Щ.

  
5��12�շ���������

  ��η�����PCtoLCD2002��������ǰһ�汾���û������̫��Ĺ��ܣ���Ϊ�Ҿ������е���Щ�����Ѿ��㹻�������ɸ�����ģ����Ҫ�ˣ��������������Ҫ�����Ƿ������ԣ�����ȥ������BUG���Լ�����һЩϸ΢֮����Ŀ�ĵ�Ȼ����׷���������������ϲ��������������Ķ�����������Ҳ�����⣬������������ͷ��βȫ������һ���˱�д��ɣ��������ޣ������˴�ʧ�ˣ������ҷ���������汾�д��ڵ�BUG���뼰ʱ�����ҡ�
    ����˵����
   1����������µ����壬�������������ѿ��ĺ�ɫ�����֣�����ǰ��ҪƯ�����ˡ�
   2������ȫ�����ʾ����������������ͨ�û��ĸ����ɻ�
   3�����������ļ�����չ����һЩBUG���������Ǽ���FON����չ���ˡ�
   4������������ģ���ݵ�һЩ��ʽBUG���������ɵ�C51��ʽ��ģ���ݻ����Ͽ���ֱ��ճ����Դ������ʹ�ö�����Ҫ�޸���
   5�������µ���ģ���ݸ�ʽ����������û������ɵĶ����Լ���Ҫ�����ݸ�ʽ
   6������Ҫ�ĸ��£�ȫ��֧�ֱ��浱ǰ���ù��ܣ��û����õ���ģ��ʽ��������״̬���ֿ����ɴ���ѡ����Ϣ���ɱ��棬��һ�δ򿪴���ʱ�����������á�
   7���������½�ͼ��ʱ���Զ�����ͼ��ģʽ��BUG
   8������������ո�ʽ����ѡ��������ɲ������հ��е���ģ���ݡ�
   9��������ÿ��������ʾ�����Ĺ��ܣ�������������ÿ����ʾ�����ݸ�������ͬʱ��������ÿ������������ʾ������
   10��������ȡģ˵����һЩ���󣬲��Ķ��˸�ʽ��
   11�����ڵ��û�ѡ��10�������ʱ�����Զ�ȥ��������ģ����ǰ�ġ�0x",�����ġ�H����ѡ��16����ʱ����Զ����ϡ�
   12���Ը����������������ȫ����Ӧ��󻯵���Ҫ����������õ�ǰ���ڲ����󣬿������ʹ�á�
   13����������Ӣ�ĵ����ֿ⹦�ܣ����Զ�����ASCII���0-127����������ֿ⣬ʹ�÷���ͬ���ɹ�������ֿ⹦�ܡ�
   14���ٴ��Ż����룬ȥ�����ֵ�����Ϣ��ʹ�����ٶ��ٿ�һЩ��
   15���������ϸ΢�ĵ����Ҽǲ����ˡ���

��Ҫע��ĵط���
  �ڲ��ԵĹ������ҷ�����һ�����⣺��WIN98��WINME�µ��û�ֱ�������ش�������ģʱ������320*320��1024*768�ĺ�����ģ������ʱ�����������ǳ��Ӵ󣬶�WIN98/WINME����64K�������������ƣ������������������޷��õ�ȫ������ģ���ݵģ���ʱ����Ҫʹ���ֿ����ɹ��ܣ�ͨ���γ�һ�������ļ����ܵõ���������ģ���ݡ�



����Ϊ�����������������Ѿ��������ˣ�������ʹ�����е㲻���㣬�������ʲô������
�ĵط������Է����ӻ�MAILѯ��



