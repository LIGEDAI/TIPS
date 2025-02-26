# 1. AXI协议
**突发长度（Burst Length）** 是在 AXI4 等总线协议中使用的一个术语，表示一次突发传输中包含的数据传输数量（即数据传输的"拍数"）。具体来说，它定义了在一次突发操作中，主设备（Master）可以连续传输的有效数据项的数量。

### 突发长度的特征

1.  **数据传输次数：**  
    突发长度决定了在一次突发操作中可以进行多少次数据传输。例如，若突发长度为 8，则在一次突发操作中可以发送 8 个数据项。
    
2.  **配合突发大小：**  
    突发长度通常与突发大小（Burst Size）结合使用。突发大小定义了每次传输的数据宽度（如 8 位、16 位、32 位等）。例如，若突发长度为 16，突发大小为 4 字节（32 位），那么总共可以传输：  
    总数据量=突发长度×突发大小=16×4 字节=64 字节
3.  **提高效率：**  
    使用突发传输可以减少控制信号的开销，提高数据传输的效率。在突发期间，主设备可以在不需要等待响应的情况下，快速传输多个数据项。
