# Vivado-bug-
记录碰到的bug
1. Vivado的异步FIFO ip核使用的时候，发现wr_data_count计数器的值并不等于真实写入数据的数量，并且它的值不随着写时钟同步变化。
[已解决]
Tips：由于设置的wr_data_count的位宽不对而引起的，使用vivado给的默认最大位宽即可，不要更改

