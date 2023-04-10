# SerenLens
[SIGIR 2023] _SerenLens_: A large ground truth dataset on serendipity-oriented recommendation. [[paper]]()

## Introduction

_SerenLens_ is our collected large ground truth dataset on people’s serendipity experiences. Here, we defined serendipity experiences based on literature: 1) having the two elements of unexpectedness and relevance in a discovery experience, and 2) the experience is positive.

The dataset uses Amazon Reviews Data (McAuley et al. 2015) as base and collects the ground truth data on serendipity by our proposed _User Semantic Mining_ approach in [paper](). Currently, the dataset contains annotated review data of two domains: **Books** and **Movies & TV**. The **Books** data have 265,037 reviews, 2,346 users, and 113,876 items. The **Movies & TV** data have 74,967 reviews, 619 users, and 23,950 movies/TV.

 ## Data Statistics
 Data statistics of each domain in _SerenLens_ dataset, more details can be found in our [paper]():
 
 |Attribute|Books|Movies & TV|
 |:----|:----:|:----:|
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
|Movies&TV|a11spsem08vixx | b001gcunzi	| 1246924800	| nicolas cage has not been in a decent film for years. you can just watch what he is in and stay away. this was not profound. this film was not intelligent. it was lame. lame ending. and lame premise. lame religious allegory and allusions. i have higher standards for thoughtful science fiction and for thrillers than this predictable nonsense. the photography also was run of the mill and so was the soundtrack. another watch it and chuck it film. no one will remember this film in a few years and it will be in the $5-$10 bin at target in a year. this, like so many films of our time, has not staying power. watching it again even one single time would produce nothing enjoyable. a real thriller stays good no matter how many times you see it. and real sci-fi makes you think, rather than give you answers.  to call this film profound is absurd. i can not believe that this was from the same director who gave us dark city. he should stick to writing his own material and stay away from these nancy boy writers who get their ideas from the church sermon, culling ideas from countless better films, and the backs of cereal boxes. ughh!	| 1 | 0 |
|Movies&TV| a1j9s070l0mvwx	| b002bwp2ik	| 1417910400	| i came across warehouse 13 by accident while looking for another dvd (i don't have cable or satellite). the premise sounded interesting so i decided to buy this (i waited until it went on sale).  i found the show to be very entertaining. i like the idea of having a "secret" warehouse (leave it to the government) with lots of "paranormal" objects. some good laughs and drama. i enjoyed it so much i went ahead and ordered seasons 2 and 3 right away (they were on sale at amazon too).  season 1 has 12 episodes; it does have english subtitles for the hearing impaired; and several "extras".	| 5	| 1 |



## Citing Us
If you feel the dataset helpful, please cite:

Fu, Z., Niu, X. and Yu, L., 2023, July. Wisdom of Crowds and Fine-Grained Learning for Serendipity Recommendations. In _Proceedings of the 46th International ACM SIGIR Conference on Research and Development in Information Retrieval_ (pp. *-*).


```  
@inproceedings{fu2023wisdom,
  author    = {Fu, Zhe and Niu, Xi(Sunshine) and Li, Yu},
  title     = {Wisdom of Crowds and Fine-Grained Learning for Serendipity Recommendations},
  booktitle = {Proceedings of the 46th International ACM SIGIR Conference on Research and Development in Information Retrieval},
  pages     = {*--*},
  publisher = {{ACM}},
  year      = {2023}
}
```
