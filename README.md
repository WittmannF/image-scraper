# Image Scraper
Selenium based image scraper on Google Images. Implementation based on [this blog post](https://towardsdatascience.com/image-scraping-with-python-a96feda8af2d). Under the folder `./images` there are some examples of small image datasets (which is actually my main goal when creating this repository - to have an easy access to some small image databases in order to experiment them in some classifiers). 

## Credits
All the credits goes to this post:
- https://towardsdatascience.com/image-scraping-with-python-a96feda8af2d

What I did here was simply organizing the code shared there as a wrapper to make it easier its usage. 

## Usage
```
In [1]: from image_scraper import search_and_download

In [2]: search_and_download?
Signature:
search_and_download(
    search_term: str,
    driver_path='chromedriver',
    target_path='./images',
    number_images=5,
)
Docstring: <no docstring>
File:      ~/projects/image-scraper/image_scraper.py
Type:      function

In [3]: search_and_download('food')
Found: 100 search results. Extracting links from 0:100
Found: 5 image links, done!
SUCCESS - saved https://images.squarespace-cdn.com/content/v1/5c5c3833840b161566b02a76/1573133725500-Y5PCN0V04I86HDAT8AT0/ke17ZwdGBToddI8pDm48kLkXF2pIyv_F2eUT9F60jBl7gQa3H78H3Y0txjaiv_0fDoOvxcdMmMKkDsyUqMSsMWxHk725yiiHCCLfrh8O1z4YTzHvnKhyp6Da-NYroOW3ZGjoBKy3azqku80C789l0iyqMbMesKd95J-X4EagrgU9L3Sa3U8cogeb0tjXbfawd0urKshkc5MgdBeJmALQKw/WBC_7095.jpg?format=2500w - as ./images/food/ce5f8e3142.jpg
SUCCESS - saved https://ichef.bbci.co.uk/news/720/cpsprodpb/BE2D/production/_112058684_gettyimages-1208790371.jpg - as ./images/food/dc045fa557.jpg
SUCCESS - saved https://www.helpguide.org/wp-content/uploads/table-with-grains-vegetables-fruit-768.jpg - as ./images/food/8eed19edb6.jpg
SUCCESS - saved https://cdn-a.william-reed.com/var/wrbm_gb_food_pharma/storage/images/publications/food-beverage-nutrition/foodnavigator.com/article/2020/04/22/coronavirus-and-obesity-doctors-take-aim-at-food-industry-over-poor-diets/10933380-3-eng-GB/Coronavirus-and-obesity-Doctors-take-aim-at-food-industry-over-poor-diets_wrbm_large.jpg - as ./images/food/93a9b5c943.jpg
SUCCESS - saved https://www.helpguide.org/wp-content/uploads/fast-foods-candy-cookies-pastries-768.jpg - as ./images/food/4569a30ac0.jpg
```
