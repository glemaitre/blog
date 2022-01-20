# scikit-learn Blog
Hosting the [scikit-learn.org](https://scikit-learn.org/stable/) blog.     
***

**Table of Contents**
- [Standards](https://github.com/scikit-learn/blog#standards)     
  - [Brand Standards](https://github.com/scikit-learn/blog#brand-standards)     
  - [Blog Standards](https://github.com/scikit-learn/blog#blog-standards)
    - [Categories & Tags](https://github.com/scikit-learn/blog#categories-&-tags)    
- [Contributing](https://github.com/scikit-learn/blog#contributing)     
  - [Installation](https://github.com/scikit-learn/blog#installation)
  - [Adding a New Post](https://github.com/scikit-learn/blog#adding-a-new-post) 
    - Setup
    - Submitting Your Blog Post
    - Formatting Your Blog Post 

&nbsp;
# Standards
This section contains scikit-learn's standards and guidelines.  <br><br>

## Brand Standards
This section contains scikit-learn's branding standards and guidelines.

### scikit-learn Color Palette
![#29ABE2 Cyan](/assets/images/brand_images/colorswatch_29ABE2_cyan.png) `RGB 41/171/226 | HEX #29ABE2 | scikit-learn Cyan`      
![#F7931E Orange](/assets/images/brand_images/colorswatch_F7931E_orange.png)  `RGB 247/147/30 | HEX #F7931E | scikit-learn Orange`     
![#9B4600 Brown](/assets/images/brand_images/colorswatch_9B4600_brown.png) `RGB 155/70/0| HEX #9B4600 | scikit-learn Brown`     

### Logo Use     
Logo. <br><br>



## Blog Standards
This section contains scikit-learn's standards and guidelines.

### Categories & Tags
Categories and Tags help us organize our blog by grouping related content to make it easier to discover.     

:warning: **NOTE:** Individual Category *(blog/category/name.md)* and Tag *(blog/tag/name.md)* pages are automatically generated by a Github Action. Please do not manually add add markdown pages.

#### Categories
Categories are broad groupings of posts. A post should have only one category. If the post could potentially fall under multiple categories, please select the one that best describes it.

*Example Categories:* Updates, Events, Team

#### Tags
Tags describe specific details of a post. They help to link related posts together and aid in user search. A post can have multiple tags or no tags. While there is no strict limit, we recommend using no more than 10 tags per post.

*Example Tags:* Sprints, Community, Open Source, New Member, Machine Learning, New Feature



&nbsp;
# Contributing
## Installation
Instructions to build and test the [scikit-learn.org/blog](https://scikit-learn.org/blog) site locally.


### Installing Ruby & Jekyll
If this is your first time using Jekyll, please follow the [Jekyll docs](https://jekyllrb.com/docs/installation/) and make sure your local environment (including Ruby) is setup correctly.


### Deployment
To run the theme locally:
1. Navigate to the theme directory and run `bundle install` to install the dependencies (if you get errors, delete Gemfile.lock and try again). 
2. Next, run `jekyll serve` or `bundle exec jekyll serve` to start the Jekyll server.
3. Visit the site in your browser via [http://localhost:4000](http://localhost:4000).

For more information, check the [Deployment Methods](https://jekyllrb.com/docs/deployment-methods/) page on the Jekyll website.

#### Theme Documentation
This blog is uses the [Minimal Mistakes Jekyll Theme](https://github.com/mmistakes/minimal-mistakes). For more information on configuration/customization, please reference the [theme documentation](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/).

&nbsp;
## Adding a New Post

### Setup
This sections contains instructions to add a new blog post to the scikit-learn blog.

Before adding a post, you must have:
- A Github account

### Submitting Your Blog Post
Refer to the [blog post template](https://github.com/scikit-learn/blog/blob/main/_posts/templates/2022-01-01-template-post.markdown).

1. First, fork the [scikit-learn/blog](https://github.com/scikit-learn/blog) repository.
2. Within your forked repository, make a copy of the [Blog Post Template](https://github.com/scikit-learn/blog/blob/main/_posts/templates/2022-01-01-template-post.markdown). 
    - Save the post in the ["_posts/"](https://github.com/scikit-learn/blog/blob/main/_posts/) folder, formatted as `YYYY-MM-DD-post-title.md`. 
    - Format your blog post using the instructions in the [Formatting Your Blog Post](https://github.com/scikit-learn/blog/blob/main/README.md#formatting-your-blog-post) section.
4. Go to Pull Requests and do a New Pull request.
5. Create a pull request.
<br>

### Formatting Your Blog Post
#### Update the Post's Front Matter
The purpose of front matter is to set variables and metadata on the site's pages.

1. **Add Post Information**
    - *title:* Add the title of your blog post in double quotes, 
        - `title: "Example Post Title"` (with quotes)
    - *date:* Add the date of posting. This helps to ensure our blog displays posts are sorted correctly and are displayed in a sequential order.
        - `date: Month Name, Day, Year` (no quotes) 
2. **Add Post Category and Tags:** Categories and tags help us organize our blog by grouping related content to make it easier to discover. Check the [Blog Standards](https://github.com/scikit-learn/blog#blog-standards) section for more information.
    - *categories:* A post should have only one category. Format categories in titlecase without dashes (Ex. "Open Source" instead of "open-source")
    - *tags:* Tags describe specific details of a post. They help to link related posts together and aid in user search.
      ![categories_tags](/assets/images/brand_images/category_tag.png)
3. **Add Featured Image**
    - *featured-image:* First, place the image in the [assets/images/posts_images/](https://github.com/scikit-learn/blog/tree/main/assets/images/posts_images) folder. Set the featured-image variable to the base image name, omiting the full path. 
        - `featured-image: image-name.png` (no quotes)
4. **Add Author Information**
    - The *postauthors* field can accomodate multiple authors. Each postauthor can use the following four variables, but only the `name` field is required.
        -  *name:* (required) 
            -  `name: Author Name` (no quotes)
        -  *website:* (optional) Link attached to author name. Can be any relevant link.
            -  `website: https://github.com` (no quotes)
        -  *email:* (optional) Appears as an email icon after author name.
            -  `email: author@email.com` (no quotes)
        -  *image:* (optional) Author headshot, appears before author name. First, place the image in the [assets/images/author_images/](https://github.com/scikit-learn/blog/tree/main/assets/images/author_images) folder. Set the image variable to the base image name, omiting the full path. 
            - `image: image-name.png` (no quotes)
        -  Single Author Post          |  Multiple Author Post
           :-------------------------:|:-------------------------:
           ![](/assets/images/brand_images/single-author-post.png)  |  ![](/assets/images/brand_images/multiple-author-post.png)
           
#### Add post content.
Format using [Markdown](https://www.markdownguide.org/). 
