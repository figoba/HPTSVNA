1.添加烧录时间格式分检的条件分支，年月日4.    11:50 2016/2/27
******************************************************************************
14:49 2016/3/2
2.修改关于工程专案删除错误的问题，旧版本是写死在程序中的数据库地址mis修正后程序不能删除数据，导致update资料失败，先改成读取txt配置文件。
3.修改打印第二张标签的时候休眠500毫秒。
4.增加烧录完成后在主页面提示相关信息。
5.增加在打印标签的动作时候，提示相关的细节步骤。
6.增加保存原始的mis的sn的，就是没有分拣过的sn，方便在烧录检测站能直接使用时间格式和流水，避免再进行对应的时间和流水的转化。Ver2.6.0.8
************************************
15:31 2016/3/2
7.发现上传到vna的详细资料中的测试结果会误判，即把OK的判定成FAIL。修改啦源程序中的判定方法。
8.修改专案设置中关于收集指定频点的测试记录中的问题，即专案管理中的设置频点单位是Hz，源代码中锁检测试文件记录中的测试频点的单位是MHZ，导致上传的数据收集不到指定频点的详细测试记录。
版本升级到Ver2.6.0.9.
**********************************************
16:04 2016/3/2
9.调试发现在正常的生产模式下，添加的itsn字段并没有插入到指定的数据库的itsn字节中。原因是第一次修改的地方是在demo模式下。后有在正常模式下做了修正。
版本升级到VerVer2.6.1.0
***********************************************
16:48 2016/3/3
10.添加当前测试Sn显示在报表选项卡中，方便子啊没有打印出条码的时候，可以用它来补打条码。
11.增加使用批处理文件强制关闭bartend。exe的进程，解决cpu利用率超高的问题。

版本升级到VerVer2.6.1.1

1.添加烧录时间格式分检的条件分支，年月日4.    11:50 2016/2/27
******************************************************************************
14:49 2016/3/2
2.修改关于工程专案删除错误的问题，旧版本是写死在程序中的数据库地址mis修正后程序不能删除数据，导致update资料失败，先改成读取txt配置文件。
3.修改打印第二张标签的时候休眠500毫秒。
4.增加烧录完成后在主页面提示相关信息。
5.增加在打印标签的动作时候，提示相关的细节步骤。
6.增加保存原始的mis的sn的，就是没有分拣过的sn，方便在烧录检测站能直接使用时间格式和流水，避免再进行对应的时间和流水的转化。Ver2.6.0.8
************************************
15:31 2016/3/2
7.发现上传到vna的详细资料中的测试结果会误判，即把OK的判定成FAIL。修改啦源程序中的判定方法。
8.修改专案设置中关于收集指定频点的测试记录中的问题，即专案管理中的设置频点单位是Hz，源代码中锁检测试文件记录中的测试频点的单位是MHZ，导致上传的数据收集不到指定频点的详细测试记录。
版本升级到Ver2.6.0.9.
**********************************************
16:04 2016/3/2
9.调试发现在正常的生产模式下，添加的itsn字段并没有插入到指定的数据库的itsn字节中。原因是第一次修改的地方是在demo模式下。后有在正常模式下做了修正。
版本升级到VerVer2.6.1.0
***********************************************
16:48 2016/3/3
10.添加当前测试Sn显示在报表选项卡中，方便子啊没有打印出条码的时候，可以用它来补打条码。
11.增加使用批处理文件强制关闭bartend。exe的进程，解决cpu利用率超高的问题。

版本升级到VerVer2.6.1.1
*************************************
12.修改打印条码的动作使用异步进程解决，如果不出标签，就可以在补打条码的窗口来 打印条码，程序不卡机。
版本升级到VerVer2.6.1.2.
17:23 2016/3/3
*************************************
9:17 2016/3/4
13.把异步打印遇到的错误信息也show出到界面上来。
*********************************************
14.添加了几个关于计数模块的子vi，还没有加入到主程序中，只把初始化计数模块的窗口添加到主页面中了。17:33 2016/3/4
*********************************************
17:53 2016/3/7
15.添加计数模块到主程序中，初步调试OK。
版本升级到VerVer2.6.1.3
*********************************************
14:58 2016/3/8
16.添加当计数板的使用寿命少于200次的时候开始弹出消息框提示。
17.添加初始化成功或者错误的提示信息框。
************************************************
18.添加主界面可以选择是否启用进行测试版的次数统计功能。
19.添加开启初始化测试版使用次数和寿命的窗口弹出时的密码验证框。
16:27 2016/3/9
版本升级到VerVer2.6.1.4
************************************************************
20.修改在专案管理模块的PING数据库名字错误的问题，会导致无法使用远程SQL，现在已经修正。
版本升级到VerVer2.6.1.5. 11:06 2016/3/11
************************************************************
21.修改计数模块单独使用一个串口进行控制。避免使用吉阳光电和IIC烧录的时候因为使用的通道数不一样而发送的命令不一样。
版本升级到版本升级到VerVer2.6.1.6. 10:04 2016/3/14
************************************************************
22.修改了在烧录EEprom的时候保存，EEpromdatesn和datecode到v_htpsVna的表单中。为在后续的检测eeprom内容的时候提供原始的资料内容。
版本没有升级。17:33 2016/3/14
*************************************************************
23.加入8路烧录和检测的延时控制的界面。11:57 2016/3/15
*************************************************************
24.修改PN改变的时候，为了测试拓展1to4的文件，把烧录的选项给成了常量一定要烧录。
25.为了测试把，上传数据的 开关改成了，不上传的常量。
18:52 2016/3/16
26.添加烧录的读写延时配置界面。19:56 2016/3/16
非加密的1拖4的烧录完成测试，能够正常使用。
以上已经恢复到正常模式。
**************************************************************
27.发现在生产SFP+10G_Lenovo_noIOQ的时候条码的时间63H，被转换成63G烧录进芯片，排查发现是高频烧录的条码时间有十进制转化成对应的烧录格式的时候出现问题。此版本已经修正问题。
版本升级到VerVer2.6.1.7  14:56 2016/3/17
******************************************************
28.修改主要的页面显示，添加保存itsn_really的字段信息。10:04 2016/3/18
29.和明光确定过加密的1to4的烧录的问题，已经能成功烧录，修改下主界面，版本没有升级。12:15 2016/3/19
版本升级到VerVer2.6.1.7  20:05 2016/3/21
******************************************************
30.修改当从MIS获得条码为空的时候，软件提示对应的信息，不进行测试。解决保存到数据库的Si和烧录Ok的记录中Itsn为空的问题。
版本升级到VerVer2.6.1.8  11:04 2016/3/28
31.验证从MIS获得的itsn包含#并且长度大于0，在第一帧中优先升级操作。16:17 2016/3/28
*******************************************************
32.增加“年月日5”的条件。把36进制转成10进制 17:45 2016/3/31
33.修改了 补印条码的 时候，关闭框口的问题。10:54 2016/4/5
***************************************************************
34.修改收集条码中分拣出来的客户流水，客户时间等全部信息。版本升级到Ver2.6.2.2. 18:25 2016/4/11
***************************************************************
35.增加华为料号失败时也能上传XML文件功能，强制MO,P/N,条码打印S/N等输入框为大写。增加保存历史MO,P/N功能。16:09 2016/5/16
***************************************************************
36.增加华为料号失败时也能上传XML文件功能，强制MO,P/N,条码打印S/N等输入框为大写。增加保存历史MO,P/N功能。解决nolabel问题。增加电脑名，执行文件路径，执行文件版本保存到XML文件中的功能。 8:38 2016/5/20 
***************************************************************
37.修正重工时对扫描进标签上的SN处理流程，由原来的对SN直接进行解析修正为从资讯数据库读取对应的条码信息，使得重测时对SN的解析和IT打印时一直，解决扫描进的SN中含有/等字符问题，同时禁止华为料号使用此重测功能。 14:36 2016/5/26
***************************************************************
38.增加完整频点XML文件生成功能（针对部分华为料号，需在配置文件中添加料号）。增加是否上传不良数据选择功能。增加不良计数功能。11:10 2016/6/7
***************************************************************
39.增加数据库连接打开后关闭功能，释放数据库连接资源，避免一直占用资讯服务器数据库资源。17:14 2016/6/12
***************************************************************
40.修改测试SCD21-SDD21的时候，可以选择减去测试夹具2X的数据。版本升级到Ver   。16:07 2016/6/24
等待使用人员验证。10:31 2016/6/25
***************************************************************
45.修改exe版本号获取方式，由直接读取exe变为读取AutoUpdate.xml里面的exe版本信息，理由：原来的方式部分电脑环境差异会读不出来。16:36 2016/7/28
***************************************************************
46.增加ILD_15测试项目，判定ILD各对之间差异是否小于15%。9:37 2016/8/16
***************************************************************
47.士龙修正关于ILD_15测试项目的部分，并上线验证OK。版本升级到Ver2.7.1.9。 17:06 2016/8/18
***************************************************************
48.士龙修正关于ILD_15测试项目的部分，并上线验证OK。ILD15%的取点数是SDD21的点数减去700个，版本没有升级。15:17 2016/8/19
***************************************************************
49.修正ILD_15规格设定，修正ILD_15规格取值错误。15:19 2016/8/26
***************************************************************
50.修正烧录SN时自动将模板里面SN后的数值初始化为20的错误，变更为仅用变换后的SN代理模板里面对应的位置。10:02 2016/9/3
***************************************************************
51.project参数设定增加机台型号，不同机台的参数可以同时存储到网络的数据库中，根据机台编号来区分。12:01 2016/9/8
***************************************************************
52.变更扫描条码测试时查询对应条码信息方式，变更前：从m_HptsVNA_t表查询，变更后：m_HptsVNA_t表中找不到就从Label_Print表查询。理由：增加了打条码工站，对应的信息在打条码时就保存到表Label_Print中去。16:28 2016/9/19
***************************************************************
53.料号设定增加是否减去夹具2X的设定，默认值为不勾选，表示需要减去夹具值；默认生成excel报告，取消需要权限。16:25 2016/9/21
***************************************************************
54.变更TDD11和TDD22共用一个测试标准为独立的两个标准，需要在project里面设定启用Impedance Filter 2。调整TDD11.txt和TDD22.txt里面的数据，变更前：TDD11.txt和TDD22.txt里面前面一半数据为一头的数据，后面一半为另一头的数据。
变更后：TDD11.txt全部数据为一个头的，TDD22.txt全部数据为另外一个头的。增加将工单号MO保存到数据库的功能。16:32 2016/9/28
***************************************************************
55.修正烧录时间的算法，变为直接取得资讯时间，无需内部转换，避免错误产生。修正TDD11_totalresult,TDD11_totalresult与实际图表显示不符。11:13 2016/10/9
***************************************************************
56.修正在SP4文件转SDD21，SDD22等文件时由于等待时间和网络延迟等造成的SP4文件还未生成完全就开始转换的错误。9:46 2016/10/27
***************************************************************
57.增加测试项目Diff Test Items平滑功能，平滑实现同matlab smooth默认函数。17:11 2016/11/7
***************************************************************
58.增加ILD_15计算时是否加上夹具值，增加ILD_15图形测试结果显示。增加测试结果TXT输出。10:36 2016/11/18
***************************************************************
59.增加测试模式选择，除正常模式外，调试和校正模式都不会上传数据到网络，只会在本地生成。增加扫描测试时条码重复检测功能。15:32 2016/12/6
***************************************************************
60.EEPROM-SN格式时（readlabel子VI）年月日3格式时已修正，不需要进制转换（原来是25进制转换），14:00 2016/12/21
***************************************************************
61.修正了程序判断年周标签类型，（对于年周且资讯返回为周日的日期，自动修正到周一，因为这边程序都是以周一作为一周的开始，
避免写EEPROM中周的码次与条码不一致），涉及VI(精简框图3、4，包括里面的读readLabel-wmg)，10:25 2016/12/23
***************************************************************
62.dealWithSNType.VI中修正（1月1日是周日的不用周加1操作）16:30 2016/12/23
***************************************************************
63.增加线别信息收集，增加工单数量报警功能，增加兼容40G开关盒选项，增加料号配置时用户验证功能。16:35 2017/1/4
***************************************************************
64.增加无日期类型时烧录算法11:47 2017/1/17
***************************************************************
65.增加2X类型的烧录处理 16:22 2017/1/23
***************************************************************
66.增加NEXT，FEXT平滑处理功能，增加NEXT FEXT生成的 txt上传到服务器，增加reportinf.txtx生成并上传到服务器。16:06 2017/2/15
***************************************************************
67.增加前站不良管控功能。11:15 2017/2/27
***************************************************************
68.增加YellowLabelPN图片设定，图片路径设定在database下的YellowLabelPN.txt下，图片放在database下的yellowLabelPN文件夹下。10:09 2017/3/9
***************************************************************
69.增加EE模式打印时流水号控制及烧录转换算法控制,优化了Webservice调用方式。14:00 2017/3/27
***************************************************************
70.修改数据库连接配置方式，设定放在figoconfig.xml里面，增加数据库密码加密功能，增加对应的加密，解密工具DES.exe。
增加MDNEXT，MDFEXT等测试项目，增加烧录校验位设定功能，增加制程条码打印功能，增加TDD11，TDD22线材截止区域域设定。9:22 2017/5/10
***************************************************************
71.增加SDD21上限规格功能，需要加在最后一列，增加异步XML生成方式。17:02 2017/06/16
***************************************************************
73.增加TDD11，22各对之间一致性检查功能。14:45 2017/06/30
***************************************************************
74.修正华为XML完整文件回传时，ILD只判断上限的错误，更改为判断绝对值小于上限。09:07 2017/07/21
***************************************************************
75.修正部分型号烧录错误。14:46 2017/08/16
***************************************************************
76.增加华为完整回传料号type 属性，属性名会附加到对应的zip文件前。
***************************************************************
77.修正日期类型为Nodate时，对应的烧录默认日期为1904年。
***************************************************************
78.增加查询T1站测试结果的功能。16:05 2017/11/20
***************************************************************
79.变更查询方式为查询资讯提供的webservice接口。14:32 2017/11/28
***************************************************************
80.变更16对时，TDD11,22的数据排列顺序，由0,1,2,3,4,5,6,7为TDD11，8,9,10,11,12,13,14,15为TDD22变更为0,1,2,3,8,9,10,11为TDD11，其余为TDD22。依据钟波的接线顺序。13:53 2017/12/13
***************************************************************
81.变更为只有以E511D开头的正常工单号才会上传华为系统。09:08 2017/12/29
***************************************************************
82.修正流水号烧录替换方式，支持从(X1)到(X99)。14:31 2018/4/10
***************************************************************
83.修正部分烧录转换时错误，增加risetime大于65时提示。8:17 2018/4/13
***************************************************************
84.增加每日点检功能。17:30 2018/5/7
