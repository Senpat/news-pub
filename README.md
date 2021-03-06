# BEST News

URL: https://senpat.github.io/news/

Repository: https://github.com/Senpat/news

Made using [NewsAPI](https://newsapi.org/) for the Capital One Summit Program.

My news site allows users to **B**rowse **E**ntertainment, **S**ports, and **T**echnology news. It has three pages: the home page, the search page, and the about page. The home page is the initial page and introduces the site. The search page is where the user can enter parameters and keywords to search the news. The about page is where users can read about how the site works.

The search results are generated by using string manipulation on the parameters and keywords to query the API in the right format. Each news article is listed by adding a section of HTML code for each article using JavaScript. Since the Top Headlines endpoint is paginated, I made a "View More" button so that the users can view the next page of articles. Each site has a banner with a color gradient. The CSS for the gradient was retrieved from uigradients.com. I also used w3schools to help me style my buttons and loader.

Users are able to filter their search in 3 different ways: 
 - By entering keywords in the search box.
 - By selecting a category out of Entertainent, Sports, and Technology.
 - By selecting the country that the news source is from. The countries were developed by adding each option to a dropdown menu using JavaScript.

The View More button is made by adding a button to the HTML if there are more articles remaining. If the button is clicked, I call the same method but increment a value that stores what page to show and pass it to the onclick function as an argument. That way, the articles of the next page are shown. To implement the loader, I add the loader HTML right before I made the API call, and remove the loader HTML right after.

To style the news articles, I made the image take up 20% of the view height and 20% of the view width. The title and time since the article was published goes to the right of the image, which I accomplished with the flex display.

To show the time since the article was published, I used a JavaScript library called moment.js which allows me to format times very easily.
