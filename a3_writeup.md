# Assignment 3 - Writeup

Assignment 3 is all about creating this natural language query system.  In order to do so, you have to write a lot of functions to retrieve infomation.  You will also have to write a function to return answers from a pattern-action list.  There is a lot of work to accomplish in this assignment, but this portion is intended for you to write about what you accomplished.

## Reflection Questions
1. In your own words describe the `search_pa_list` function.
A: It takes a source (What the user typed) and it tries to understand what the user is asking for based on the patterns of the questions provided. In this situation, it is trying to understand any questions regarding movies(name, director, title, etc.). It should return any information about movies that the user specifically requested. 

2. What movie did you add to the `movies.py` file?  What year was it made? Any specific reason you added that movie?
A: I added the movie Cruella, created in the year 2021. I just added it because it was the first movie it came in mind, for it is a movie that I saw recently

3. What pattern / action did you add to the paList data structure?  Why do you think that is a useful pattern / action?
A: (str.split("how long ago was % made"), year_by_title)
It can be useful to know what movies are old and which movies aren't

4. What is chatbot would you create that would be like this?  Describe why you would create it and what it would do.
A: I would create a chatbot that would find locations of restaurants based on the user's information given. This could be created because it will be useful for people to find places they would like to go and not get lost.

5. What was the most difficult portion of this assignment?
A: Putting all conditions in the search_pa_list function and creating a new pattern/making code accept new pattern

6. Did you write a new assert for your pattern action?
A: I added another insert regarding the movie i added to the list
    assert sorted(
        search_pa_list(["how", "long", "ago", "was", "cruella", "made"])
    ) == sorted(["2 years ago"]), "failed search_pa_list test 4"
it was mostly a test to see if the movie and new pattern I added worked with the code
I also edited the title after year assert so the movie I added won't make the code see error
assert sorted(title_after_year(["1990"])) == sorted(
        ["boyz n the hood", "dead again", "the crying game", "flirting", "malcolm x", "cruella"]
    ), "failed title_after_year test"
