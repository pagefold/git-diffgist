git-diffgist
============

Automatically create a GitHub Gist from a git diff, with a summary of files changed.

### Usage ###
```bash
git diffgist SHA1 SHA2        # diff between two commits
git diffgist master myBranch  # diff between master and myBranch's HEAD
git diffgist master           # diff between master and current HEAD
```

### Install ###
```bash
sudo gem install jist  # if not already installed
sudo curl -o $(dirname $(which git))/git-diffgist https://raw.github.com/pagefold/git-diffgist/master/git-diffgist && sudo chmod 755 $(dirname $(which git))/git-diffgist

# Note that the install will overwrite an existing file at this location.
# It will attempt to install next to your environment's git at git-diffgist.
```

### Requirements ###
* [GitHub account](http://github.com)
* [jist gem](https://github.com/ConradIrwin/jist)
* [Git](http://git-scm.com/)


### Additional Notes ###
When creating gists, the command will store timestamp-versioned text files under a _.gitdiffs_ directory in your home directory.

This has the benenfit of setting the filename of the Gist as well as an archive with timestamps for when each gist was generated.


## License ##
Copyright (C) 2012 Brandon McKinney

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
