# ExpertSearch

To run the code, run the following command from `ExpertSearch` (tested with Python2.7 on MacOS and Linux):

`gunicorn server:app -b 127.0.0.1:8095` 

The site should be available at http://localhost:8095/

# Live Demo

There will not be live demos scheduled for this project, unless a reviewer is absolutely unable to get the code running on their own. Instead, there is a video available to view with UIUC school credentials at https://drive.google.com/file/d/10HNOJZRPQ2lLqYDfIC213dDoGAChQEv7/view?usp=sharing 
It should be noted that the page that is shown in the first part is the current ExpertSearch website http://timan102.cs.illinois.edu/expertsearch/. The added functionality program is run locally through my personal computer. We can see how the new functionality allows users the convenience of not having to click the "Load More" button, while the program is simultaneously not burdensome by loading all the results at once.

If reviewers want to personally run the code, they can simply download the repository and run it per the instructions above (may need to pip install some packages) to achieve/replicate the results. If issues occur, please message/email me as the author and we will get things sorted out. Please not that you should absolutely use Linux or MacOS, as gunicorn will not run in Windows, and install Python 2.7 (not any Python3 distributions). I personally used Ubuntu in developing this project.

If, for any reason, one needs to access the ExpertSearch Github, it can be found at https://github.com/CS410Fall2020/ExpertSearch/ 

# Explanation of how code utilizes system

The code's primary functionality is in-built to the system, such that if pushed to the master project of ExpertSearch, it would integrate perfectly with no issues. The simple change made was to add a function that checked for if the user's screen was close to the bottom; if so, it would scroll automatically. One caveat of this approach is that it will not work until the user first clicks the "Load More" button. However, after contemplating, it was decided this was actually the correct functionality; if a user clicks load more, we can assume that only then they want to see more results. Perhaps some users may only wish to see the first five results and not be bombarded with an excessive number of results until they click the "Load More" button themselves.
