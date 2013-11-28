B: Specify features

We want to add a useful feature called article merging.  When there are multiple bloggers on one site, the authors may write more than one article on the same topic and say similar things.  The user will be able to visit the article view, and, if they are an admin, there should be a form on that article’s edit page that allows an administrator to enter in the ID of another article to merge the current article with.  When this happens, we want to preserve both articles’ content, but merge them together into one article.

Note: Before merging articles you should verify that both specified articles exist, and that they are not the same article.

 

Scenarios: To do this properly, we want to keep the following in mind:

 

    A non-admin cannot merge articles.

    When articles are merged, the merged article should contain the text of both previous articles.

    When articles are merged, the merged article should have one author (either one of the authors of the original article).  

    Comments on each of the two original articles need to all carry over and point to the new, merged article.

    The title of the new article should be the title from either one of the merged articles.

Start by writing cucumber scenarios for the above behaviors. You will probably want to put them in separate feature files. You may add them to the existing feature files. Over the rest of part 1 and all of part 2 we will make these go green. 
