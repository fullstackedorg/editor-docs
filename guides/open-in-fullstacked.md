# Open in FullStacked

If you use git to version your project,
you can easily share your project with a link that will open directly try to open your repository in FullStacked!

## Deep Link

After installing the FullStacked Editor and opening it once, the FullStacked Editor will associate the `fullstacked://` scheme to open in the FullStacked Editor.
To open your git repository project, add your git url after this scheme and open it through any browser.

Make sure to use the git repo url ending with `.git`.

```
fullstacked://[git/repo/url.git]

Example:
fullstacked://https://github.com/fullstackedorg/editor-sample-demo.git
```

### Using the npm CLI

If you are using the FullStacked Editor through the npm CLI installation, 
you can do the same by launching fullstacked with the git repository url as argument.

```shell
fullstacked [git/repo/url.git]

or

npx @fullstacked/editor -- [git/repo/url.git]
```

## Share page

If your recipient doesn't have the FullStacked Editor installed beforehand, the `fullstacked://` url will bring them into a dead end.
To share your project in a more fashionably, use the https://fullstacked.org/share page to send your project deep link.
Simply add your git url in the query parameters.

```
https://fullstacked.org/share?git=[git/repo/url.git]

Example:
https://fullstacked.org/share?git=https://github.com/fullstackedorg/editor-sample-demo.git
```
Try it out  
https://fullstacked.org/share?git=https://github.com/fullstackedorg/editor-sample-demo.git

## Markdown Button

You can even add an "Open in FullStacked" button to your `README` page to allow people to directly open your project in the FullStacked Editor.
To do so, create an image link with the share page url.

```
[![Open in FullStacked]([image/url])](share/page?git=[git/repo/url.git])

Example:
[![Open in FullStacked](https://raw.githubusercontent.com/fullstackedorg/website/main/open-in-fullstacked.svg)](https://fullstacked.org/share?git=https://github.com/fullstackedorg/editor-sample-demo.git)
```

Try it out  
[![Open in FullStacked](https://raw.githubusercontent.com/fullstackedorg/website/main/open-in-fullstacked.svg)](https://fullstacked.org/share?git=https://github.com/fullstackedorg/editor-sample-demo.git)

## Extra parameters

You can also add some extra parameters to make sure sharing your project goes as expected.
To add extra parameters, simply add them as query parameters to the git repository url.

```
Deep Link
fullstacked://[git/repo/url.git]?title=Demo

Share Page
https://fullstacked.org/share?git=[git/repo/url.git]?title=Demo
```

### Available parameters

| Param Name | default |
| -------- | ------- |
| `title` | username/repo-name |


