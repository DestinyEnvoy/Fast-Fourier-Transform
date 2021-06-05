# 说明

- 用Verlilog硬件描述语言对[DIT-FFT](https://en.wikipedia.org/wiki/Cooley-Tukey_FFT_algorithm)分模块进行功能设计，最终仿真实现16点复数的FFT。
- 用测试信号对本设计进行测试，并分析计算结果和matlab计算结果的误差。
- 详细说明见报告[./report/main.pdf](https://github.com/DestinyEnvoy/Fast-Fourier-Transform/report/main.pdf)

```
├─matlab    : matlab 程序，对比verilog和理论计算误差
├─report    : 设计的报告文件
├─sim       : test bench 测试文件
│      butterfly_tb.v   : 蝶形运算单元的test bench 测试文件
│      fft_top_tb.v     : FFT单元的test bench 测试文件
│      
└─unit      : 功能单元设计
        butterfly.v     : 蝶形运算单元
        fft_ctrl_sm.v   : 控制单元
        fft_top.v       : 顶层文件
        mem_32x16.v     : 缓冲存储单元(RAM)
        read_addr_lut.v : 地址发生存储单元
        w_lut.v         : 旋转因子存储单元
        

```

# 致谢

- [ameyk1/Fast-Fourier-Transform](https://github.com/ameyk1/Fast-Fourier-Transform)
- [StickCui/XDUthesis-personal](https://github.com/StickCui/XDUthesis-personal)
