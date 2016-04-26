

Today, I'm going to introduce [git-remote-dropbox](https://github.com/anishathalye/git-remote-dropbox) , a tool that let you turn your DropBox into a real git server.

Maybe you are wondering why doing that, while there are a bunch of free services as bitbucket and others that offer unlimited private repositories ?

That's true, but wouldn't be good if we keep our regular files and codes together in one place :sunglasses: ? All in One backup ! 

Some free services do limit the number of collaborators, so by using this tool, you can add as much as you want !

Let's start : 

- [*] Installing using [PyPI](https://pypi.python.org/pypi)

```
	pip install git-remote-dropbox.
```  

-  Go to [app console](https://www.dropbox.com/developers/apps/create) in your DropBox account
-  Create a Dropbox API app with full access to all files and file types
-  Generate the OAuth 2 token and create a new file

```json
{
    "token": "-----------"
}
```


-  Save it to ~/.git-remote-dropbox.json 





To clone repositories in folders mounted in your Dropbox, you can run:


```
git clone "dropbox://path/to/repo"
```

To add a remote to an existing local repository, you can run:

```
git remote add origin "dropbox://path/to/repo"
```


Enjoy :thumbsup:
