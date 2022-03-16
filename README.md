# Seattle Snowmass Website Source

Please submit PR's if you'd like to see anything new here! The website can currently be found here
[http://seattlesnowmass2021.net](http://seattlesnowmass2021.net).


# Running this locally

The following command is used to run this locally:

```bash
docker run --rm -it -v {repo-location}:/gitrepo -p 4001:4000 jekyll/jekyll:4.0 bash -c \"'cd /gitrepo; jekyll serve --incremental --force_poll'\"
```

Once it is up and running you can point your browser at `http://localhost:4001`. When you make modifications it should automatically update the site in the container without you having to re-run anything. The initial start up is slow: lots of ruby assets need to be downloaded.

If you are using `vscode` you can just run the task _jekyll serve (docker)_. This version of the command will also cache gems between runs, making startup after the initial startup significantly faster.