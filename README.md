# BaiduMapJsWebGLApiTrackAnimation

修复此demo的问题：http://lbsyun.baidu.com/index.php?title=jspopularGL/guide/trackAnimation


## SEO

百度地图 WEBGL jsapi 轨迹动画  几内亚湾

## 解决方式

替换该项目中的TrackAnimation.min.js文件即可

## 问题复现

当轨迹坐标点定位不准、点漂移等原因导致轨迹无法正常展示，最明显的现象就是坐标定位到(0,0)，几内亚湾

官方demo地址：http://lbsyun.baidu.com/jsdemo.htm#webgl6_1

当坐标点不准时，比如:
> [
                {
                    "lng":119.25881831563,
                    "lat":35.314176621282
                },
                {
                    "lng":119.25887102983,
                    "lat":35.314183842875
                },
                {
                    "lng":119.25897932488,
                    "lat":35.31419867766
                },
                {
                    "lng":119.25893777,
                    "lat":35.314192985451
                },
                {
                    "lng":119.25890980813,
                    "lat":35.314189155092
                },
                {
                    "lng":119.25890503023,
                    "lat":35.31418850058
                },
                {
                    "lng":119.25890999669,
                    "lat":35.314189180922
                },
                {
                    "lng":119.25891274845,
                    "lat":35.314189557876
                },
                {
                    "lng":119.2588964312,
                    "lat":35.314187322616
                },
                {
                    "lng":119.25889157615,
                    "lat":35.314186657527
                },
                {
                    "lng":119.25890217239,
                    "lat":35.314188109092
                },
                {
                    "lng":119.25890982524,
                    "lat":35.314189157434
                },
                {
                    "lng":119.2589139425,
                    "lat":35.314189721444
                },
                {
                    "lng":119.25887476876,
                    "lat":35.314184355078
                },
                {
                    "lng":119.25890047359,
                    "lat":35.314187876376
                },
                {
                    "lng":119.25894169659,
                    "lat":35.314193523326
                },
                {
                    "lng":119.25896284471,
                    "lat":35.314196420225
                },
                {
                    "lng":119.25894177782,
                    "lat":35.314193534454
                },
                {
                    "lng":119.25892917039,
                    "lat":35.314191807443
                },
                {
                    "lng":119.25902073091,
                    "lat":35.314204349252
                },
                {
                    "lng":119.25888896586,
                    "lat":35.314186299945
                },
                {
                    "lng":119.25896609802,
                    "lat":35.314196865862
                },
                {
                    "lng":119.25883718638,
                    "lat":35.314179206524
                },
                {
                    "lng":119.2588765371,
                    "lat":35.314184597324
                },
                {
                    "lng":119.2631996379,
                    "lat":35.314774913689
                },
                {
                    "lng":119.2639552859,
                    "lat":35.311876051673
                },
                {
                    "lng":119.26798233232,
                    "lat":35.29841751598
                },
                {
                    "lng":119.26795776552,
                    "lat":35.286993148287
                },
                {
                    "lng":119.26708419553,
                    "lat":35.283356381164
                },
                {
                    "lng":119.27155902211,
                    "lat":35.269739651301
                },
                {
                    "lng":119.27393337201,
                    "lat":35.251653771169
                },
                {
                    "lng":119.27619656155,
                    "lat":35.23505243829
                },
                {
                    "lng":119.27632486109,
                    "lat":35.230163984119
                },
                {
                    "lng":119.28047275098,
                    "lat":35.219913565289
                },
                {
                    "lng":119.28564436166,
                    "lat":35.213580065234
                },
                {
                    "lng":119.29055344385,
                    "lat":35.201231961931
                },
                {
                    "lng":119.29362700269,
                    "lat":35.195125337211
                },
                {
                    "lng":119.29743297297,
                    "lat":35.184209636288
                },
                {
                    "lng":119.2955843901,
                    "lat":35.174497751846
                },
                {
                    "lng":119.2961370131,
                    "lat":35.164407850412
                },
                {
                    "lng":119.29746408328,
                    "lat":35.152499735471
                },
                {
                    "lng":119.29794740923,
                    "lat":35.143371113923
                },
                {
                    "lng":119.30073475134,
                    "lat":35.142575437356
                },
                {
                    "lng":119.30676006444,
                    "lat":35.139902026067
                },
                {
                    "lng":119.30415573814,
                    "lat":35.135099676495
                },
                {
                    "lng":119.30296276616,
                    "lat":35.129497430032
                },
                {
                    "lng":119.30851539747,
                    "lat":35.127207246904
                },
                {
                    "lng":119.31909002548,
                    "lat":35.125202793808
                },
                {
                    "lng":119.31859389896,
                    "lat":35.126038837693
                },
                {
                    "lng":119.31862113689,
                    "lat":35.125859361261
                },
                {
                    "lng":119.31877902566,
                    "lat":35.125800446762
                },
                {
                    "lng":119.31874103623,
                    "lat":35.125379218441
                },
                {
                    "lng":119.31151518443,
                    "lat":35.126585603546
                },
                {
                    "lng":119.30946930493,
                    "lat":35.127046820986
                },
                {
                    "lng":119.29927820016,
                    "lat":35.131114101016
                },
                {
                    "lng":119.29826152459,
                    "lat":35.131395240081
                },
                {
                    "lng":119.29133305823,
                    "lat":35.134363263517
                },
                {
                    "lng":119.29114649669,
                    "lat":35.133865123503
                },
                {
                    "lng":119.29114085231,
                    "lat":35.13385818571
                },
                {
                    "lng":119.29114010597,
                    "lat":35.133857268344
                },
                {
                    "lng":119.29115787271,
                    "lat":35.133879106216
                },
                {
                    "lng":119.29057703889,
                    "lat":35.134677609776
                },
                {
                    "lng":119.29775576911,
                    "lat":35.139352812362
                },
                {
                    "lng":119.30092949125,
                    "lat":35.142590947244
                },
                {
                    "lng":119.29761855763,
                    "lat":35.152506148037
                },
                {
                    "lng":119.2962884646,
                    "lat":35.164448473365
                },
                {
                    "lng":119.29577752597,
                    "lat":35.175206264213
                },
                {
                    "lng":119.29753848496,
                    "lat":35.182902310064
                },
                {
                    "lng":119.29762242295,
                    "lat":35.184000655735
                },
                {
                    "lng":119.29594496511,
                    "lat":35.188681533244
                },
                {
                    "lng":119.29382340909,
                    "lat":35.195158967872
                },
                {
                    "lng":119.28763595151,
                    "lat":35.208658634096
                },
                {
                    "lng":119.28606058137,
                    "lat":35.213215376715
                },
                {
                    "lng":119.27689643591,
                    "lat":35.228035860166
                },
                {
                    "lng":119.27623181691,
                    "lat":35.235771591746
                },
                {
                    "lng":119.27284880535,
                    "lat":35.265556402045
                },
                {
                    "lng":119.26829881565,
                    "lat":35.279515333317
                },
                {
                    "lng":119.26693237689,
                    "lat":35.282812799728
                },
                {
                    "lng":119.26800020049,
                    "lat":35.291666100102
                },
                {
                    "lng":119.27303480826,
                    "lat":35.292036092549
                },
                {
                    "lng":119.27278178728,
                    "lat":35.294227583855
                },
                {
                    "lng":119.2719090037,
                    "lat":35.294165034047
                },
                {
                    "lng":119.27191557511,
                    "lat":35.294165515095
                },
                {
                    "lng":119.2719850294,
                    "lat":35.294170597431
                },
                {
                    "lng":119.26863853296,
                    "lat":35.294024486983
                },
                {
                    "lng":119.26799145753,
                    "lat":35.294009584839
                },
                {
                    "lng":119.26545803482,
                    "lat":35.294632252058
                },
                {
                    "lng":119.2659933279,
                    "lat":35.294645631786
                },
                {
                    "lng":119.26504722259,
                    "lat":35.294621895406
                },
                {
                    "lng":119.26464823918,
                    "lat":35.302086764625
                },
                {
                    "lng":119.26287944614,
                    "lat":35.307506714039
                },
                {
                    "lng":119.26265177467,
                    "lat":35.307797691724
                },
                {
                    "lng":119.26334885906,
                    "lat":35.314792548248
                },
                {
                    "lng":119.25902003478,
                    "lat":35.314204253901
                },
                {
                    "lng":119.25906268378,
                    "lat":35.314210095511
                },
                {
                    "lng":119.2589224113,
                    "lat":35.31419088155
                },
                {
                    "lng":119.2589311087,
                    "lat":35.314192072962
                },
                {
                    "lng":119.25892446312,
                    "lat":35.314191162618
                },
                {
                    "lng":119.25892928527,
                    "lat":35.31419182318
                },
                {
                    "lng":119.25893585598,
                    "lat":35.314192723262
                },
                {
                    "lng":119.25888035408,
                    "lat":35.314185120217
                },
                {
                    "lng":119.25883442411,
                    "lat":35.314178828103
                },
                {
                    "lng":119.26223571972,
                    "lat":35.314643718102
                },
                {
                    "lng":119.2634988683,
                    "lat":35.313003129775
                },
                {
                    "lng":119.26251352673,
                    "lat":35.307843225394
                },
                {
                    "lng":119.26483783486,
                    "lat":35.300067602689
                },
                {
                    "lng":119.26783263257,
                    "lat":35.298944888828
                },
                {
                    "lng":119.26799431192,
                    "lat":35.296084151507
                },
                {
                    "lng":119.26877358011,
                    "lat":35.296121463878
                }]
                
                
                
                
                

就会出现偏移到(0,0)的问题

