Movie Info 0.5
==============
By Kim Bratzel 2014
--------------

This program goes through your movie collection (folders or files within a directory) and gathers extra information about each movie using a third party API.

It generates a nice looking webpage which includes a sortable table containing each movie's title, cover image, etc. It also creates coverflow style view of your movie collection ordered by IMDB Rating.

...This is still very much a work in progress.


Change Log
--------------
 - 0.6 (Coming Soon)
    - Erroneous Title Correction
    - CoverFlow View
    - Unit Tests
 - 0.5 Stable Release
 - 0.5 Beta


Dependencies
--------------

 - python 2.7+
 - jinja2 - http://jinja.pocoo.org/ - sudo pip install jinja2


Usage Examples
--------------

    python ./src/main.py -d ./tests/testMovieDirectory     -html -limit 500    > example-output.html
    python ./src/main.py -d ./tests/testMovieDirectory     -l 900              > example-output.txt

    python ./src/main.py -dir /Volumes/My_Book/Movies      -html               > example-output.html
    python ./src/main.py -dir /Volumes/KIM/TV Shows        -html -limit 500    > example-output.html

    python ./src/main.py -h (help)
    python ./src/main.py -v (version)

The most important part is the directory where your movies are stored.
They can be files or folders within that directory.



Example Output
--------------

You can generate some example HTML output by running the following script:

    ./generate_example_html.sh

Tests
--------------

To run the tests (these aren't finished yet...) run this script:

    ./run_tests.sh


ToDo
--------------

 - Finish erroneous title correction

 - Make HTML Pretty
 - Finish writing the unit tests
 - Use an alternative API for failed lookups
 - Much more...


Contact
--------------

Get in touch: kimbratzel.com
