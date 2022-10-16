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

<embed src="/images/deepfakes/cdn/vidtimit_cdn.html"  width=600 height=600/>

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

<embed src="/images/deepfakes/cdn/DeepfakeTIMIT_cdn.html"  width=600 height=600/>

# UADFV

total: 98 videos

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

<embed src="/images/deepfakes/cdn/UADFV_cdn.html"  width=600 height=600/>

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

<embed src="/images/deepfakes/cdn/FaceForensics++_cdn.html"  width=600 height=600/>

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

<embed src="/images/deepfakes/cdn/Celeb-DF-v2_cdn.html"  width=600 height=600/>

# DFD Google

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

<embed src="/images/deepfakes/cdn/DFD_cdn.html"  width=600 height=600/>


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

<embed src="/images/deepfakes/cdn/dfdc_preview_cdn.html"  width=600 height=600/>

# DFDC:

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

<embed src="/images/deepfakes/cdn/dfdc_cdn.html"  width=600 height=600/>


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

<embed src="/images/deepfakes/cdn/DeeperForensics-1.0_cdn.html" width=600 height=600/>

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



<embed src="/images/deepfakes/cdn/FFIW10K_cdn.html" width=600 height=600/>

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

<embed src="/images/deepfakes/cdn/Wilddeepfake_cdn.html" width=600 height=600/>
