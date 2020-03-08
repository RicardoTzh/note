## shell变量

1. 变量类型由被赋值变量决定。如下，若a，b传入数字，则可以正常执行。否则需要使用expr执行计算。

   ```shell
   #!/bin/bash
   
   declare - i c
   read a
   read b
   c=$a+$b
   echo $c
   ```

   