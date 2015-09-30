# Setup

```ShellSession
$ hugo new site notes-to-self
$ cd notes-to-self
$ hugo new about.md

```

# Workflow

## New post

```ShellSession
$ hugo new post/some-title.md
$ vi content/post/some-title.md
$ hugo undraft post/some-title.md
```

Watch progress with

```ShellSession
$ hugo server --buildDrafts --watch
```

## Publish on Github Pages

`hugo shell` should not be running when you do this:

```ShellSession
$ hugo
$ git add . && git commit -m "blah" && git push
$ git subtree push --prefix=public git@github.com:bertvv/notes-to-self.git gh-pages
```

See <https://gohugo.io/tutorials/github-pages-blog/>

# Tricks

## Source code

```
{{< highlight LANGUAGE>}}
source code
{{< /highlight >}}
```

For a list of supported languages, see <http://pygments.org/languages/>

