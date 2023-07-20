# SerenLens
[SIGIR 2023] This repository contains the annotated dataset _SerenLens_ introduced in our full paper in SIGIR2023 _Wisdom of Crowds and Fine-Grained Learning for Serendipity Recommendations_. [[paper]](https://dl.acm.org/doi/10.1145/3539618.3591787)

## Introduction

_SerenLens_ is our collected large ground truth dataset on people’s serendipity experiences. Here, we defined serendipity experiences based on literature: 1) having the two elements of unexpectedness and relevance in a discovery experience, and 2) the experience is positive.

The dataset uses Amazon Reviews Data (McAuley et al. 2015) as base and collects the ground truth data on serendipity by our proposed _User Semantic Mining_ approach in [paper](https://dl.acm.org/doi/10.1145/3539618.3591787). Currently, the dataset contains annotated review data of two domains: **Books** and **Movies & TV**. The **Books** data have 265,037 reviews, 2,346 users, and 113,876 items. The **Movies & TV** data have 74,967 reviews, 619 users, and 23,950 movies/TV.

 ## Data Statistics
 Data statistics of each domain in _SerenLens_ dataset, more details can be found in our [paper](https://dl.acm.org/doi/10.1145/3539618.3591787):
 
 |Attribute|Books|Movies & TV|
 |----|:----:|:----:|
 |**User invloved in the reviews of serendipity**|**2,346**|**619**|
 |Items involved in the reviews of serendipity|2,227|634|
 |Other reviews involved for the involved users|262,691|74,253|
 |**Total reviews involved**|**265,037**|**74,967**|
 |**Total items involved**|**113,876**|**23,950**|

 ## Data Format
Datasets of each domain share a uniform format:
 
 * user_id: the id number of users.
 * item_id: the id number of items.
 * timestamp: the timestamp of the review.
 * review: the content of the reviews.
 * rating: the 5-star rating of the reviews.
 * label: the label of serendipitous feelings for the reviews, 0 denotes not serendipitous feeling, 1 denotes serendipitous feeling.
 
| File name | Description | Number of record |
| ---- | ---- | ---- |
| SerenLens_Books.csv | Serendipity data of Amazon book reviews | 265,037 |
| SerenLens_Movies.csv | Serendipity data of Amazon movie & TV reviews | 74,967 |


 ## Data Examples
Examples of annotated review data in two different domains:

| Domain | user_id |	item_id	| timestamp |	review	| rating	| label |
| ---- | ---- | ---- | ---- | ---- | :----: | :----: |
|Books| a10e3f50diujee	| 0061148512	| 1196899200	| i have always loved this book.  plath's literature is exceptional, in my opinion.  but the reason i bought this copy, even though i already own one, is because there are a few of plath's sketches included in this edition.  it may seem insignificant, but for someone who likes plath, this should be quite a treat!	| 5	| 0 |
|Books| a9owlc66j3584	| 0151015392	| 1339718400	| this is one of my all time favorite books. i stumbled upon the paperback in the high school library and was immediately hooked. this book is funny, dramatic, scary and even romantic. when they made the movie i was incredibly excited. this is probably the best adaptation i have ever seen. read this book, watch the movie and then repeat. I highly recommend it.	| 5	| 1 |
|Movies&TV| a18758s1puyidt	| b005lzw9fs	| 1344211200	| i can imagine how the plans for this one went:  let's pay someone a few dollars to write some stupid story, pay the "actors" a few bucks each to attempt to act and fail at it, shoot the same scenes over and over with really dumb effects, and wonder how many times the viewer will fast forward it just to get to the end.	| 1	 | 0 |
|Movies&TV| a1j9s070l0mvwx	| b002bwp2ik	| 1417910400	| i came across warehouse 13 by accident while looking for another dvd (i don't have cable or satellite). the premise sounded interesting so i decided to buy this (i waited until it went on sale).  i found the show to be very entertaining. i like the idea of having a "secret" warehouse (leave it to the government) with lots of "paranormal" objects. some good laughs and drama. i enjoyed it so much i went ahead and ordered seasons 2 and 3 right away (they were on sale at amazon too).  season 1 has 12 episodes; it does have english subtitles for the hearing impaired; and several "extras".	| 5	| 1 |



## Citing us
If you feel the dataset helpful, please cite:

Fu, Z., Niu, X. and Yu, L., 2023, July. Wisdom of Crowds and Fine-Grained Learning for Serendipity Recommendations. In _Proceedings of the 46th International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. *-*).


```  
@inproceedings{10.1145/3539618.3591787,
author = {Fu, Zhe and Niu, Xi and Yu, Li},
title = {Wisdom of Crowds and Fine-Grained Learning for Serendipity Recommendations},
year = {2023},
isbn = {9781450394086},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
url = {https://doi.org/10.1145/3539618.3591787},
doi = {10.1145/3539618.3591787},
booktitle = {Proceedings of the 46th International ACM SIGIR Conference on Research and Development in Information Retrieval},
pages = {739–748},
numpages = {10},
location = {Taipei, Taiwan},
series = {SIGIR '23}
}
```
