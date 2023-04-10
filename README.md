# SerenLens
[SIGIR 2023] _SerenLens_: A large ground truth dataset on serendipity-oriented recommendation. [[paper]]()

## Introduction

_SerenLens_ is our collected large ground truth dataset on people’s serendipity experiences. The dataset uses Amazon Reviews Data (McAuley et al. 2015) as base and collects the ground truth data on serendipity by our proposed _User Semantic Mining_ approach in [paper](). Currently, the dataset contains annotated review data of two domains: **Books** and **Movies & TV**. The **Books** data have 265,037 reviews, 2,346 users, and 113,876 items. The **Movies & TV** data have 74,967 reviews, 619 users, and 23,950 movies/TV.

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

## Citing us
If you feel the datasets helpful, please cite:

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
