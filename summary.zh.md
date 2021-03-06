
# {{ 页面标题 }}

本章描述了如何在网络数据包中编码应用程序数据. 与本书前面描述的协议不同,您可以将其视为处理*消息*,这些转变过程*数据*. 诸如视频,静止图像和音频之类的多媒体数据类型正在越来越多地推动该领域的发展. 

第一个问题是表示格式化,其中问题是格式化应用程序计算的不同类型的数据,使得它们可以通过网络传输并由接收器正确解释. 数据类型 (如整数,浮点数,字符串,数组和结构) 必须以某种可理解的方式进行编码. 这涉及在机器和网络字节顺序之间进行转换以及线性化复合数据结构. 我们概述了表示格式的设计空间,并讨论了设计空间中不同点的四种特定机制: XDR,ASN.1,NDR和日益重要的XML. 

第二个问题是压缩,它涉及减少传输不同类型数据所需的带宽. 压缩算法可以是无损的或有损的,有损算法最适合于图像和视频数据. JPEG,MPEG和MP3都分别对静止图像,视频和音频数据使用有损压缩协议. 视频压缩和编码格式 (例如MPEG系列标准) 不断发展,以满足在可用带宽限制内对更高质量的需求. 

## 进一步阅读

我们推荐的本章阅读清单包括两篇文章,分别概述了JPEG和MPEG标准. 它们的主要价值在于解释塑造标准的各种因素. 我们还推荐关于接收器驱动的分层多播的论文,作为系统设计方法的一个很好的例子,包括多播,拥塞控制和视频编码的问题. 

-   华莱士,G. K. JPEG静态图片压缩标准. ACM的通讯*1991年4月34 (1) : 30-44. *Le Gall,D. MPEG: 多媒体应用的视频压缩标准. 

-   ACM的通讯*1991年4月34 (1) : 46-58. *McCanne,S.,V. Jacobson和M. Vetterli. 

-   接收器驱动的分层组播. *SIGCOMM '96研讨会论文集,*1996年9月第117-130页. 
