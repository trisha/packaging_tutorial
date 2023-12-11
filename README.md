# Example PyPi Package

This is a simple example package from the [tutorial](https://packaging.python.org/en/latest/tutorials/packaging-projects/) from [pypi](https://pypi.org/). You can use
[GitHub-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
to write your content.

- More info on .toml: https://packaging.python.org/en/latest/guides/writing-pyproject-toml/


# Confirming that it works
Once it gets uploaded (FYI the test server occassionaly deletes packages so would have to reupload), enter the below in Terminal/iTerm2:

`ipython` to enter virtual environment
`!python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps example-package-trishie` the ! in front is an escape character that tells iPython that it's a terminal command
`!python3` to enter interpreter
```from example_package_trishie import example
example.add_one(2)``` should return 3!

The instructions above for testing are slightly different when on main network instead of test network but the differences are described in the pet project tutorial in the [Next Steps](https://packaging.python.org/en/latest/tutorials/packaging-projects/#next-steps) section.