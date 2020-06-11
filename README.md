# BOOK GENRE CLASSIFICATION BY ITS COVER USING MULTI-VIEW LEARNING APPROACH

### Abstract
An interesting topic in visual analysis is to determine the genre of a book by
its cover. The book cover is the very first communication to the reader which shapes
the reader’s expectation about the type of the book. Each book cover is carefully
designed by the cover designers and typographers to convey the visual representation
of its content. In this study, we explore several different deep learning approaches for
predicting the genre from the cover image alone, such as MobileNet V1, MobileNet V2,
ResNet50, Inception V2. Moreover, we add an extra modality by extracting text from
the cover image. We explore some simple text classification algorithms such as LSTM
and Universal Sentence Decoder. Moreover, we focus on model concatenation based on
of two best performing models on cover image and text. Finally, we propose the use
of [deep canonical correlation analysis(DCCA)](http://www.jmlr.org/proceedings/papers/v28/andrew13.pdf) to jointly learn the features from two modalities:
image and text, then use a support vector machine classifier to predict the genre of the
book. Overall, concatenation of two models yields the best result. However, our analysis
revealed the weakness of these models for solving this task on our used dataset. Our
results suggest that solving this task to a satisfactory level needs significant efforts and
much-more accurate dataset.

### Dataset
To evaluate the proposed study, we use the [BookCover30 dataset](https://github.com/uchidalab/book-dataset) proposed by
[Iwana and Uchida 2016](https://arxiv.org/pdf/1610.09204.pdf). This dataset contains 57,000 book cover images divided into
30 genres. 

| | | |
|-|-|-|
| Arts & Photography | Biographies & Memoirs | Business & Money |
| Calendars | Children's Books | Christian Books & Bibles |
| Comics & Graphic Novels | Computers & Technology | Cookbooks, Food & Wine |
| Crafts, Hobbies & Home | Engineering & Transportation | Health, Fitness & Dieting |
| History | Humor & Entertainment | Law |
| Literature & Fiction | Medical Books | Mystery, Thriller & Suspense |
| Parenting & Relationships | Politics & Social Sciences | Reference |
| Religion & Spirituality | Romance | Science & Math |
| Science Fiction & Fantasy | Self-Help | Sports & Outdoors |
| Teen & Young Adult | Test Preparation | Travel |

