# Page-Rank-Visualization-using-Python-3
This program crawls a web site and pulls a series of pages into the database, recording the links between pages. 

spider.py: to crawl a website and retrieve two pages.  If you restart the program again and tell it to crawl more pages, it will not re-crawl any pages already in the database.  Upon restart it goes to a random non-crawled page and starts there.  So each successive run of spider.py is additive.

spdump.py: This shows the number of incoming links, the old page rank, the new page rank, the id of the page, and the url of the page.  The spdump.py program only shows pages that have at least one incoming link to them.

Once you have a few pages in the database, you can run Page Rank on the pages using the sprank.py program.  You simply tell it how many Page Rank iterations to run.
For each iteration of the page rank algorithm it prints the average change per page of the page rank.   The network initially is quite  unbalanced and so the individual page ranks are changing wildly. But in a few short iterations, the page rank converges.  You  should run prank.py long enough that the page ranks converge.

If you want to visualize the current top pages in terms of page rank, run spjson.py to write the pages out in JSON format to be viewed in a web browser.

You can view this data by opening the file force.html in your web browser.This shows an automatic layout of the nodes and links.  You can click and 
drag any node and you can also double click on a node to find the URL that is represented by the node.

Note: Windows has difficulty in displaying UTF-8 characters in the console so for each console window you open, you may need
to type the following command before running this code:

    chcp 65001
