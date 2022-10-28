---
title: 'Deepfakes Datasets'
date: 2022-10-15
permalink: /posts/2022/10/deepfakes-datasets/
tags:
  - deepfakes
  - forgery
  - datasets
---

This is the first post in this blog.
To start, I will introduce the datasets that I used in my work.
These are the datasets that have been used in the literature to train deepfakes models.

------

# VIDTIMIT

Videos have a constant format
- width 512
- height 384
-	fps 25
- frames (54-240)

Identities: 43 with each 10 videos.

Sentences: 10 sentences per identity (one per video)
with the following 2 sentences for every person:
-	“She had your dark suit in greasy wash water all year.”
-	“Don't ask me to carry an oily rag like that.”

The other 8 sentences are randomly selected from a corpus of 238 minus the previous two sentences.
<details>
    <summary>Click me</summary>
  ```json
  [
    "si1010",
    "si1024",
    "si1039",
    "si1084",
    "si1088",
    "si1099",
    "si1105",
    "si1116",
    "si1175",
    "si1178",
    "si1179",
    "si1199",
    "si1218",
    "si1230",
    "si1264",
    "si1265",
    "si1279",
    "si1303",
    "si1360",
    "si1364",
    "si1375",
    "si1386",
    "si1398",
    "si1400",
    "si1425",
    "si1454",
    "si1463",
    "si1469",
    "si1473",
    "si1474",
    "si1490",
    "si1502",
    "si1538",
    "si1539",
    "si1541",
    "si1542",
    "si1543",
    "si1544",
    "si1553",
    "si1555",
    "si1566",
    "si1573",
    "si1587",
    "si1624",
    "si1640",
    "si1653",
    "si1664",
    "si1669",
    "si1714",
    "si1718",
    "si1729",
    "si1735",
    "si1746",
    "si1808",
    "si1825",
    "si1829",
    "si1848",
    "si1894",
    "si1899",
    "si1909",
    "si1933",
    "si1988",
    "si2005",
    "si2016",
    "si2028",
    "si2030",
    "si2084",
    "si2093",
    "si2098",
    "si2099",
    "si2104",
    "si2120",
    "si2128",
    "si2149",
    "si2168",
    "si2169",
    "si2171",
    "si2172",
    "si2173",
    "si2183",
    "si2203",
    "si2222",
    "si2247",
    "si2255",
    "si2270",
    "si2284",
    "si2294",
    "si2299",
    "si458",
    "si469",
    "si475",
    "si522",
    "si545",
    "si548",
    "si549",
    "si565",
    "si569",
    "si634",
    "si635",
    "si639",
    "si649",
    "si673",
    "si728",
    "si730",
    "si734",
    "si745",
    "si756",
    "si768",
    "si770",
    "si818",
    "si824",
    "si833",
    "si838",
    "si839",
    "si844",
    "si860",
    "si869",
    "si908",
    "si909",
    "si911",
    "si912",
    "si913",
    "si923",
    "si943",
    "si992",
    "si995",
    "sx10",
    "sx100",
    "sx101",
    "sx102",
    "sx103",
    "sx104",
    "sx109",
    "sx11",
    "sx110",
    "sx113",
    "sx115",
    "sx118",
    "sx119",
    "sx1195",
    "sx12",
    "sx124",
    "sx126",
    "sx13",
    "sx133",
    "sx134",
    "sx138",
    "sx139",
    "sx14",
    "sx140",
    "sx1625",
    "sx184",
    "sx185",
    "sx188",
    "sx189",
    "sx19",
    "sx190",
    "sx191",
    "sx192",
    "sx193",
    "sx194",
    "sx199",
    "sx20",
    "sx200",
    "sx203",
    "sx205",
    "sx208",
    "sx209",
    "sx214",
    "sx216",
    "sx223",
    "sx224",
    "sx228",
    "sx229",
    "sx23",
    "sx230",
    "sx25",
    "sx274",
    "sx275",
    "sx278",
    "sx279",
    "sx28",
    "sx280",
    "sx281",
    "sx282",
    "sx283",
    "sx284",
    "sx289",
    "sx29",
    "sx290",
    "sx293",
    "sx295",
    "sx298",
    "sx299",
    "sx304",
    "sx306",
    "sx313",
    "sx314",
    "sx318",
    "sx319",
    "sx320",
    "sx34",
    "sx36",
    "sx364",
    "sx365",
    "sx368",
    "sx369",
    "sx370",
    "sx371",
    "sx372",
    "sx373",
    "sx374",
    "sx379",
    "sx380",
    "sx383",
    "sx385",
    "sx388",
    "sx389",
    "sx394",
    "sx396",
    "sx4",
    "sx403",
    "sx404",
    "sx408",
    "sx409",
    "sx410",
    "sx43",
    "sx44",
    "sx48",
    "sx49",
    "sx5",
    "sx50",
    "sx8",
    "sx9",
    "sx94",
    "sx95",
    "sx98",
    "sx99"
  ]
  ```
</details>


total: 430 videos

label
- **REAL** 430 (100.00 %)

fold
- **real** 430 (100.00 %)


|   label | fold   |   count |   percent |
|--------:|:-------|--------:|----------:|
|       0 | real   |     430 |       100 |





<div style="position:relative;overflow:hidden;width:100%;">
<embed src="/images/deepfakes/cdn/vidtimit_cdn.html"  width="100%" height="100%" style="position:absolute;top:0;left:0;bottom:0;right:0;"/>
</div>

# DeepfakeTIMIT

total: 1070 videos

label
- **FAKE** 640 (59.81 %)
- **REAL** 430 (40.19 %)

fold
- **real** 430 (40.19 %)
- **fake_HQ** 320 (29.91 %)
- **fake_LQ** 320 (29.91 %)


|   label | fold    |   count |   percent |
|--------:|:--------|--------:|----------:|
|       0 | real    |     430 |     40.19 |
|       1 | fake_HQ |     320 |     29.91 |
|       1 | fake_LQ |     320 |     29.91 |

<embed src="/images/deepfakes/cdn/DeepfakeTIMIT_cdn.html"  width="100%" height="100%"/>

---

# UADFV

total: 98 videos

generated with FakeAPP

label
- **REAL** 49 (50.00 %)
- **FAKE** 49 (50.00 %) 

fold
- **youtube** 49 (50.00 %)
- **FakeAPP** 49 (50.00 %)


|   label | fold    |   count |   percent |
|--------:|:--------|--------:|----------:|
|       0 | youtube |      49 |        50 |
|       1 | FakeAPP |      49 |        50 |

<embed src="/images/deepfakes/cdn/UADFV_cdn.html"  width="100%" height="100%"/>

# FaceForensics++: 

total: 6000 videos

label
- **FAKE** 5000 (83.33 %)
- **REAL** 1000 (16.67 %)

fold
- **youtube** 1000 (16.67 %)
- **Deepfakes** 1000 (16.67 %)
- **Face2Face** 1000 (16.67 %)
- **FaceShifter** 1000 (16.67 %)
- **FaceSwap** 1000 (16.67 %)
- **NeuralTextures** 1000 (16.67 %)

split
- **train** 4320 (72.00 %)
- **test** 840 (14.00 %)
- **val** 840 (14.00 %)

|   label | fold           | split   |   count |   percent |
|--------:|:---------------|:--------|--------:|----------:|
|       0 | youtube        | test    |     140 |      2.33 |
|       0 | youtube        | train   |     720 |     12    |
|       0 | youtube        | val     |     140 |      2.33 |
|       1 | Deepfakes      | test    |     140 |      2.33 |
|       1 | Deepfakes      | train   |     720 |     12    |
|       1 | Deepfakes      | val     |     140 |      2.33 |
|       1 | Face2Face      | test    |     140 |      2.33 |
|       1 | Face2Face      | train   |     720 |     12    |
|       1 | Face2Face      | val     |     140 |      2.33 |
|       1 | FaceShifter    | test    |     140 |      2.33 |
|       1 | FaceShifter    | train   |     720 |     12    |
|       1 | FaceShifter    | val     |     140 |      2.33 |
|       1 | FaceSwap       | test    |     140 |      2.33 |
|       1 | FaceSwap       | train   |     720 |     12    |
|       1 | FaceSwap       | val     |     140 |      2.33 |
|       1 | NeuralTextures | test    |     140 |      2.33 |
|       1 | NeuralTextures | train   |     720 |     12    |
|       1 | NeuralTextures | val     |     140 |      2.33 |

<embed src="/images/deepfakes/cdn/FaceForensics++_cdn.html"  width="100%" height="100%"/>

<details>
    <summary>Identities per split (json)</summary>

{
  "train": [1,2,5,6,7,8,9,10,11,13,14,16,17,18,19,20,21,22,25,27,28,30,31,32,33,34,37,38,39,40,41,43,45,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,65,66,67,68,69,70,71,72,74,75,76,77,79,80,81,82,83,85,86,87,88,89,90,92,93,94,95,96,97,98,99,100,101,103,105,107,108,109,110,111,112,113,117,118,119,120,121,122,123,124,125,127,129,130,131,132,133,136,137,139,140,143,144,146,147,148,149,150,151,152,153,155,156,160,162,163,164,165,166,167,168,171,172,173,174,177,178,179,180,181,182,183,184,185,187,188,189,191,193,194,195,196,197,199,200,201,202,203,204,205,206,207,208,209,210,211,212,213,215,216,217,218,221,222,224,225,226,228,229,230,231,232,234,235,236,237,238,239,240,241,242,243,244,246,247,248,250,251,252,253,256,258,259,260,262,264,265,266,267,268,269,270,271,272,274,275,276,277,279,281,282,283,285,286,287,289,290,291,292,293,294,295,296,297,298,300,301,302,303,304,305,307,309,310,311,312,313,315,317,318,320,322,323,324,326,327,328,329,330,331,332,333,334,335,336,337,338,339,340,341,343,344,345,346,348,351,353,355,356,357,359,360,361,363,365,366,368,372,373,374,375,377,378,382,383,385,387,390,391,392,393,394,395,396,397,398,400,401,403,405,406,407,408,409,410,411,412,413,414,415,417,424,426,427,428,430,431,432,433,434,435,436,437,438,439,441,442,444,446,447,448,449,450,451,456,457,458,459,460,461,463,464,466,469,473,474,475,476,477,478,481,484,486,487,489,490,491,495,496,497,498,499,500,501,502,503,504,505,506,508,509,510,512,513,515,516,518,519,520,522,523,524,525,526,528,530,531,532,533,534,535,536,537,539,540,541,542,543,544,545,546,547,549,551,553,554,555,556,559,561,562,563,568,569,570,572,573,574,575,576,577,578,580,581,582,587,588,590,591,592,593,594,596,598,600,601,602,603,604,605,609,610,611,613,614,615,616,618,619,620,621,624,626,627,628,629,631,635,636,637,639,641,642,643,644,645,646,648,651,652,653,654,655,657,658,659,662,663,665,667,671,673,674,676,677,678,679,680,681,684,685,686,687,688,689,690,692,693,694,696,697,698,699,700,703,704,708,709,710,711,712,713,715,716,717,718,719,721,722,723,726,728,730,733,734,735,736,737,738,740,743,744,747,748,749,750,751,752,753,754,756,757,758,760,761,763,764,765,766,767,769,770,771,772,773,774,776,778,780,781,782,783,784,785,786,787,788,789,790,791,792,795,796,797,798,799,800,802,803,804,805,806,808,809,810,811,813,814,815,819,822,825,826,828,829,830,831,833,835,836,838,839,840,841,843,844,845,846,848,849,850,853,854,856,858,859,860,861,863,864,866,867,869,870,871,872,873,874,876,877,878,879,881,882,883,884,885,886,887,888,889,891,892,893,894,897,899,901,902,903,905,907,908,910,911,913,914,916,918,920,921,928,929,930,931,934,935,936,937,938,940,941,942,943,944,946,948,950,952,954,957,959,960,961,962,963,964,965,966,967,968,969,972,975,976,977,978,981,983,984,985,986,987,988,989,990,993,994,996,997,998,999],
  "test": [0,3,12,15,24,26,29,35,36,44,47,48,73,78,102,114,128,135,138,141,142,154,158,161,169,170,176,186,190,214,219,220,227,233,249,255,257,278,280,288,306,308,314,319,321,347,352,358,367,371,376,379,380,381,384,386,388,389,399,404,418,420,421,422,423,425,429,445,452,454,462,467,479,480,485,488,494,507,517,521,527,529,550,552,579,607,608,623,625,630,633,634,650,660,661,669,670,675,682,683,691,695,701,705,706,707,714,724,725,731,732,739,741,755,759,801,812,821,842,847,851,855,862,865,868,880,896,906,917,919,924,932,945,949,953,955,970,973,974,995],
  "val": [4,23,42,46,64,84,91,104,106,115,116,126,134,145,157,159,175,192,198,223,245,254,261,263,273,284,299,316,325,342,349,350,354,362,364,369,370,402,416,419,440,443,453,455,465,468,470,471,472,482,483,492,493,511,514,538,548,557,558,560,564,565,566,567,571,583,584,585,586,589,595,597,599,606,612,617,622,632,638,640,647,649,656,664,666,668,672,702,720,727,729,742,745,746,762,768,775,777,779,793,794,807,816,817,818,820,823,824,827,832,834,837,852,857,875,890,895,898,900,904,909,912,915,922,923,925,926,927,933,939,947,951,956,958,971,979,980,982,991,992]
}

</details>


<img src="/images/deepfakes/ff++/faceforensics++.svg" width="100%" style="height: auto;"/>

# Celeb-DF-v1:

total: 1203 videos

label
- **1** 795 (66.08 %)
- **0** 408 (33.92 %)

fold
- **Celeb-synthesis** 795 (66.08 %)
- **YouTube-real** 250 (20.78 %)
- **Celeb-real** 158 (13.13 %)

split
- **train** 1103 (91.69 %)
- **test** 100 (8.31 %)


|   label | fold            | split   |   count |   percent |
|--------:|:----------------|:--------|--------:|----------:|
|       0 | Celeb-real      | train   |     150 |     12.47 |
|       0 | Celeb-real      | test    |       8 |      0.67 |
|       0 | YouTube-real    | train   |     220 |     18.29 |
|       0 | YouTube-real    | test    |      30 |      2.49 |
|       1 | Celeb-synthesis | train   |     733 |     60.93 |
|       1 | Celeb-synthesis | test    |      62 |      5.15 |

<embed src="/images/deepfakes/cdn/Celeb-DF-v1_cdn.html" width="100%" height="100%"/>

identities:

total = 15
```json
[0, 1, 2, 3, 4, 6, 7, 8, 9, 10, 11, 12, 13, 16, 17]
```

missing = 3
```
[5, 14, 15]
```

# Celeb-DF-v2:

total: 6529 videos

label
- **FAKE** 5639 (86.37 %)
- **REAL** 890 (13.63 %)

fold
- **Celeb-synthesis** 5639 (86.37 %)
- **Celeb-real** 590 (9.04 %)
- **YouTube-real** 300 (4.59 %)

split
- **train** 6011 (92.07 %)
- **test** 518 (7.93 %)


|   label | fold            | split   |   count |   percent |
|--------:|:----------------|:--------|--------:|----------:|
|       0 | Celeb-real      | train   |     482 |      7.38 |
|       0 | Celeb-real      | test    |     108 |      1.65 |
|       0 | YouTube-real    | train   |     230 |      3.52 |
|       0 | YouTube-real    | test    |      70 |      1.07 |
|       1 | Celeb-synthesis | train   |    5299 |     81.16 |
|       1 | Celeb-synthesis | test    |     340 |      5.21 |

<embed src="/images/deepfakes/cdn/Celeb-DF-v2_cdn.html"  width="100%" height="100%"/>

**Identities**

total = 15
```json
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 16, 17, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61]
```

missing = 3
```
[14, 15, 18]
```

**Celebrities** 

total: 59 

Gender:
male (56.8%)
female (43.2%)

age: 
>=60 (8.5%); 
[50, 60] (30.5%); 
40s (26.6%)
30s (28.0%)
<30 (6.4%) 

Ethnic groups:
Asians (5.1%)
African Americans (6.8%) 
Caucasians (88.1%)

# Deep Fake Detection Dataset

DFD: The Google/Jigsaw DeepFake detection dataset

total: 3431 videos

label
- **1** 3068 (89.42 %)
- **0** 363 (10.58 %)

fold
- **DeepfakeDetection** 3068 (89.42 %)
- **actors** 363 (10.58 %)

scenes
- **outside_talking_pan_laughing** 291 (8.48 %)
- **walk_down_hall_angry** 276 (8.04 %)
- **outside_talking_still_laughing** 268 (7.81 %)
- **kitchen_pan** 263 (7.67 %)
- **talking_against_wall** 260 (7.58 %)
- **podium_speech_happy** 257 (7.49 %)
- **exit_phone_room** 246 (7.17 %)
- **walking_outside_cafe_disgusted** 239 (6.97 %)
- **walking_down_street_outside_angry** 229 (6.67 %)
- **kitchen_still** 225 (6.56 %)
- **talking_angry_couch** 198 (5.77 %)
- **secret_conversation** 182 (5.30 %)
- **hugging_happy** 180 (5.25 %)
- **walking_and_outside_surprised** 139 (4.05 %)
- **walking_down_indoor_hall_disgust** 121 (3.53 %)
- **meeting_serious** 57 (1.66 %) 

| scene                             | count real |   percent real || count fake | percent fake |
|:----------------------------------|-----------:|---------------:||-----------:|-------------:|
| exit_phone_room                   |         28 |           0.82 ||        218 |         6.35 |
| hugging_happy                     |         16 |           0.47 ||        164 |         4.78 |
| kitchen_pan                       |         27 |           0.79 ||        236 |         6.88 |
| kitchen_still                     |         26 |           0.76 ||        199 |         5.8  |
| meeting_serious                   |          4 |           0.12 ||         53 |         1.54 |
| outside_talking_pan_laughing      |         28 |           0.82 ||        263 |         7.67 |
| outside_talking_still_laughing    |         27 |           0.79 ||        241 |         7.02 |
| podium_speech_happy               |         28 |           0.82 ||        229 |         6.67 |
| secret_conversation               |         18 |           0.52 ||        164 |         4.78 |
| talking_against_wall              |         27 |           0.79 ||        233 |         6.79 |
| talking_angry_couch               |         22 |           0.64 ||        176 |         5.13 |
| walk_down_hall_angry              |         28 |           0.82 ||        248 |         7.23 |
| walking_and_outside_surprised     |         15 |           0.44 ||        124 |         3.61 |
| walking_down_indoor_hall_disgust  |         15 |           0.44 ||        106 |         3.09 |
| walking_down_street_outside_angry |         28 |           0.82 ||        201 |         5.86 |
| walking_outside_cafe_disgusted    |         26 |           0.76 ||        213 |         6.21 |

<embed src="/images/deepfakes/cdn/DFD_cdn.html"  width="100%" height="100%"/>


# DFDC-preview:

total: 5250 videos

label
- **FAKE** 4119 (78.46 %)
- **REAL** 1131 (21.54 %)

fold
- **method_A** 3975 (75.71 %)
- **original_videos** 1131 (21.54 %)
- **method_B** 144 (2.74 %)

split
- **train** 4473 (85.20 %)
- **test** 777 (14.80 %)

|   label | fold            | split   |   count |   percent |
|--------:|:----------------|:--------|--------:|----------:|
|       1 | method_A        | train   |    3501 |     66.69 |
|       1 | method_A        | test    |     474 |      9.03 |
|       1 | method_B        | train   |     117 |      2.23 |
|       1 | method_B        | test    |      27 |      0.51 |
|       0 | original_videos | train   |     855 |     16.29 |
|       0 | original_videos | test    |     276 |      5.26 |

<embed src="/images/deepfakes/cdn/dfdc_preview_cdn.html"  width="100%" height="100%"/>

# DFDC:

Facebook DeepFake Detection Challenge Dataset (DFDC)

total: 128154 videos

label
- **REAL**  23654 (81.54 %)
- **FAKE**  104500 (18.45 %)

split
- **train** 119154 (92.98 %)
- **test** 5000 (3.90 %)
- **val** 4000 (3.12 %)

|   label | split   |   count |   percent |
|--------:|:--------|--------:|----------:|
|       0 | test    |  2500   | 1.95      |
|       0 | train   |  19154  | 14.95     |
|       0 | val     |  2000   | 1.56      |
|       1 | test    |  2500   | 1.95      |
|       1 | train   |  100000 | 78.03     |
|       1 | val     |  2000   | 1.56      |

<embed src="/images/deepfakes/cdn/dfdc_cdn.html"  width="100%" height="100%"/>


# DeeperForensics-1.0

total: 59475 videos

label
- **REAL** 48475 (81.50 %)
- **FAKE** 11000 (18.50 %)

split
- **train** 41452 (69.70 %)
- **test** 12368 (20.80 %)
- **val** 5655 (9.51 %)

|   label | split   |   count |   percent |
|--------:|:--------|--------:|----------:|
|       0 | test    |   10157 |     17.08 |
|       0 | train   |   33719 |     56.69 |
|       0 | val     |    4599 |      7.73 |
|       1 | test    |    2211 |      3.72 |
|       1 | train   |    7733 |     13    |
|       1 | val     |    1056 |      1.78 |

<embed src="/images/deepfakes/cdn/DeeperForensics-1.0_cdn.html" width="100%" height="100%"/>


**Perturbation**
There are 7 types of [distortions](https://github.com/EndlessSora/DeeperForensics-1.0/tree/master/perturbation) with 5 intensity (levels):
(transmission errors, compression, etc.) 
- CS: Color Staturation	Change
- BW: Local Block Wise Distortion
- CC: Color Contrast Change
- GB: Gaussian blur
- GNC: White Gaussian Noise in Color Components
- JPEG: JPEG Compression	
- VC: Video Compression Rate Change


<img src="/images/deepfakes/df1/7perturbations.jpg" width="100%" style="height: auto;"/>

Additionally, 3 distortion are created by mixing respectively 2, 3 and 4 of the above distortions, ie. {CS, BW}, {CS, BW, CC}, {CS, BW, CC, GB}.

<img src="/images/deepfakes/df1/mixed.jpg" width="100%" style="height: auto;"/>

Each forgery video is then augmented using:
- 1 original forgery
- 1 forgery postprocessed with the original frames by color matching, warping, affine transformation, etc.
- 1 random distortion at a random level
- 5 randomly choosen distortion at level-{1, 2, 3, 4, 5}
- 3 mix-{2, 3, 4} distortions

total: 11 videos per forgery


**Identities**:
All the 11000 FAKE videos are created using **source** videos from DeeperForensics-1.0 dataset and the **target** videos are the 1000 pristine videos from FaceForensics++ dataset.

When keeping only the test 140 identities of FaceForensics++ used as source for the DeeperForensics-1.0 dataset, we get the following:
label
- **FAKE** 1540 = 140 * 11 (100.00 %)

label
- **1** 1540 (100.00 %)

split
- **train** 1100 (71.43 %)
- **test** 330 (21.43 %)
- **val** 110 (7.14 %)

manipulation
- **end to end** 140 (9.09 %)
- **reenact postprocess** 140 (9.09 %)
- **end to end random level** 140 (9.09 %)
- **end to end level 1** 140 (9.09 %)
- **end to end level 2** 140 (9.09 %)
- **end to end level 3** 140 (9.09 %)
- **end to end level 4** 140 (9.09 %)
- **end to end level 5** 140 (9.09 %)
- **end to end mix 2 distortions** 140 (9.09 %)
- **end to end mix 3 distortions** 140 (9.09 %)
- **end to end mix 4 distortions** 140 (9.09 %)

# FFIW10K

total: 19976 videos

label
- **REAL** 9988 (50.00 %)
- **FAKE** 9988 (50.00 %)

fold
- **web** 19976 (100.00 %)

split
- **train** 16000 (80.10 %)
- **test** 3476 (17.40 %)
- **val** 500 (2.50 %)


|   label | fold   | split   |   count |   percent |
|--------:|:-------|:--------|--------:|----------:|
|       0 | web    | train   |    8000 |     40.05 |
|       0 | web    | val     |     250 |      1.25 |
|       0 | web    | test    |    1738 |      8.7  |
|       1 | web    | train   |    8000 |     40.05 |
|       1 | web    | val     |     250 |      1.25 |
|       1 | web    | test    |    1738 |      8.7  |



<embed src="/images/deepfakes/cdn/FFIW10K_cdn.html" width="100%" height="100%"/>

# Wilddeepfake

total: 7312 videos

label
- **REAL** 3805 (52.04 %)
- **FAKE** 3507 (47.96 %)

split
- **train** 6506 (88.98 %)
- **test** 806 (11.02 %)

|   label | split   |   count |   percent |
|--------:|:--------|--------:|----------:|
|       1 | test    |     410 |      5.61 |
|       1 | train   |    3097 |     42.36 |
|       0 | test    |     396 |      5.42 |
|       0 | train   |    3409 |     46.62 |


<embed src="/images/deepfakes/cdn/Wilddeepfake_cdn.html" width="100%" height="100%"/>


# KoDF

total: 237824 videos

label
- **1** 175660 (73.86 %)
- **0** 62164 (26.14 %)

fold
- **fo** 61867 (26.01 %)
- **crowdsourcing** 52964 (22.27 %)
- **dffs** 37080 (15.59 %)
- **dfl** 34464 (14.49 %)
- **fsgan** 23888 (10.04 %)
- **audio-driven** 18361 (7.72 %)
- **studio** 9200 (3.87 %)

sex
- **F** 130502 (54.87 %)
- **M** 107322 (45.13 %)

|   label | fold          | sex   |   count |   percent |
|--------:|:--------------|:------|--------:|----------:|
|       0 | crowdsourcing | F     |   27023 |     11.36 |
|       0 | crowdsourcing | M     |   25941 |     10.91 |
|       0 | studio        | F     |    4600 |      1.93 |
|       0 | studio        | M     |    4600 |      1.93 |
|       1 | fo            | F     |   32615 |     13.71 |
|       1 | fo            | M     |   29252 |     12.3  |
|       1 | audio-driven  | F     |    6870 |      2.89 |
|       1 | audio-driven  | M     |   11491 |      4.83 |
|       1 | dfl           | F     |   21910 |      9.21 |
|       1 | dfl           | M     |   12554 |      5.28 |
|       1 | dffs          | F     |   22575 |      9.49 |
|       1 | dffs          | M     |   14505 |      6.1  |
|       1 | fsgan         | F     |   14909 |      6.27 |
|       1 | fsgan         | M     |    8979 |      3.78 |

<embed src="/images/deepfakes/cdn/KoDF_cdn.html" width="100%" height="100%"/>

Acronyms:
- **fo**: FOMM
- **dffs**: FaceSwap
- **dfl**: DeepFaceLab
- **fsgan**: FSGAN
- **audio-driven**: AudioDriven : {ATFHP, Wav2Lip}


| Age           | Count | %      |
|---------------|-------|--------|
| ∼19           | 5     | 1.24   |
| 20∼29         | 205   | 50.87  |
| 30∼39         | 106   | 26.30  |
| 40∼49         | 61    | 15.14  |
| 50∼59         | 19    | 4.71   |
| 60∼           | 7     | 1.74   |

| Sex           | Count | %      |
|---------------|-------|--------|
| Female        | 205   | 50.87  |
| Male          | 198   | 49.13  |

| Location      | Count | %      |
|---------------|-------|--------|
| Crowdsourcing | 353   | 87.59  |
| Studio        | 50    | 12.41  |

