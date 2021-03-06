# LBS气泡地图 {#concept_glz_t4f_vdb .concept}

**说明：** LBS气泡地图只可用于**Quick BI专业版**。

您如果已经阅读过[仪表板概述](cn.zh-CN/快速入门/报表制作/仪表板概述.md#)和[仪表板基本操作](cn.zh-CN/快速入门/报表制作/仪表板基本操作/仪表板基本操作.md#)，那么本章将为您介绍如何创建一个LBS气泡地图。如果您还需要对数据集做进一步的编辑，或者想重新创建一个数据集，请参阅[创建数据集](cn.zh-CN/快速入门/数据建模/管理数据集/创建数据集.md#)。

LBS气泡地图与[气泡地图](cn.zh-CN/快速入门/报表制作/仪表板图表制作/气泡地图.md#)类似，都是以一个地图轮廓为背景，用附着在地图上面的气泡来反映数据的大小，而且，还可以切换地图的底图样式，例如高德地图、谷歌地图和GeoQ直观地显示国家或地区的相关数据指标大小和分布范围。如展示各地旅游景点的客流量，或者展示各地区的人均收入等。

LBS气泡地图是由地理区域和LBS气泡大小构成的。地理区域由数据的维度或者经纬度决定，如省份；LBS气泡的大小由数据的度量决定，如运输成本，订单数量等。

## LBS气泡地图须知 {#section_ezb_x4f_vdb .section}

LBS气泡地图的地理区域最多只能取1个维度，并且维度类型必须为地理信息或者经纬度，如区域，省，城市等；LBS气泡大小区域最少取1个，并且最多取5个度量。

以下场景均以company\_sales\_record数据集和常规仪表板为例。

**场景示例：用LBS气泡地图展示各省的订单金额和利润金额。**

1.  登录Quick BI控制台。
2.  单击**数据集**，进入数据集管理页面。
3.  找到company\_sales\_record数据集，单击**新建仪表板**，进入仪表板编辑页面。
    -   如果您使用的是**标准版**或者**高级版**，页面会自动跳转到常规仪表板编辑页面。
    -   如果您使用的是**专业版**，需要您手动选择进入**常规模式**或者**全屏模式**。以下示例以**常规模式**为例。
4.  在仪表板配置区，单击**LBS气泡地图**图标。
5.  在数据标签页，选择需要的维度字段和度量字段。

    在维度列表中，找到**省份**，并将其添加到地理区域中；在度量列表中，找到**订单金额**和**利润金额**，并将依次添加到LBS气泡大小区域中，如下图所示。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/9145/15342423921870_zh-CN.png)

6.  单击**更新**，更新图表。
7.  在样式标签页可更改图表的标题，布局和某一个字段的显示格式，如下图所示。

    ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/9145/15342423921871_zh-CN.png)

    -   在**布局**中，您可以设置地图的底图样式、缩放地图的大小和调整地图的经纬度。例如将底图设置为**GeoQ**，更新后的图表如下图所示。

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/9145/15342423921872_zh-CN.png)

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/9145/15342423921873_zh-CN.png)

    -   在**系列设置**中，将订单金额的小数位数设置为2位，更新后的图表显示如下。

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/9145/15342423921874_zh-CN.png)

        ![](http://static-aliyun-doc.oss-cn-hangzhou.aliyuncs.com/assets/img/9145/15342423921876_zh-CN.png)

8.  单击**保存**，保存该仪表板。

    在图表右上方，选择**更多操作** \> **删除**，可删除当前图表。


有关各地区详细信息对照表请参见：[http://docs-aliyun.cn-hangzhou.oss.aliyun-inc.com/assets/attach/54802/cn\_zh/1534146495493/%E5%9C%B0%E5%8C%BA%E8%AF%A6%E6%83%85%E4%BF%A1%E6%81%AF%E8%A1%A8.xlsx](http://docs-aliyun.cn-hangzhou.oss.aliyun-inc.com/assets/attach/48322/cn_zh/1534241743586/%E5%90%84%E5%9C%B0%E5%8C%BA%E8%AF%A6%E7%BB%86%E4%BF%A1%E6%81%AF%E5%AF%B9%E7%85%A7%E8%A1%A8.xls)。

