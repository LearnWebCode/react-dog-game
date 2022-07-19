# [Play the Game on GitHub Pages](https://learnwebcode.github.io/react-dog-game/)

You can learn how to code this game step by step by checking out the [YouTube video](https://www.youtube.com/watch?v=nmbpZ-RJaLY) it was created for.

The `npm run build` task will create a folder named dist, but GitHub Pages would need the folder to be named "docs" instead. Instead of manually changing the folder name, you can [configure Vite to use a different build output folder](https://vitejs.dev/config/build-options.html#build-outdir).

Also, Vite formats the paths to load your JS and CSS assets using absolute URLs instead of relative. Meaning, they start with a forward slash, so they will work perfectly at the root of a domain, but if your project lives in a sub-folder of a domain, like GitHub pages for example, you'll need to go into your build folder's index.html file and manually adjust the path to your assets to be relative. I'm sure there's a way to automate that change in the `vite.config.js` file but I'm a Vite noob and couldn't find out how to do that in my 45 seconds of research.
