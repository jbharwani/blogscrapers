# blogscrapers

Need to install scrapy and selenium
```
	pip install scrapy
	pip install selenium
```

This package provides python scripts that can be used to scrape every archived blog posts from blogspot, wordpress, and typepad. The scripts make the assumption that the sites follow a certain HTML structure. The following sites are examples of compatible blogs. 

blogspot - "http://autismschmatism.blogspot.com/"
wordpress - "https://rhemashope.wordpress.com/"
typepad - "http://lizditz.typepad.com/i_speak_of_dreams/archives.html"


What is important is the xpath for the archives on the main page and the HTML tags for each post. Just modify the xpath in the scraper file to navigate to the archive links and scrape parts. Firefox and the firebug package will be very useful to this.

To scrape the blog x into a file titled "data.json":
	1. Open appropriate scraper and make changes as commented on the top of the 	file
	2. Go to the command line and navigate to the correct directory
	3. Run the following command
		scrapy runspider scraper.py -o data.json
