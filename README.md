# Academic Webpage

A repo for building [my website](https://aditya-shirwatkar.github.io) using Hugo and host it on github pages

## Dependencies for building

- [Hugo](https://gohugo.io/)
- [Go](https://go.dev/)

## Updating Commands

```bash
git add .
git commit -m "Making Changes"
git push -u origin master

hugo # Generate the website inside the public directory
cd public
git add .
git commit -m "Build website"
git push origin master
cd ..
```

## Credits

- [Hugo Academic Theme](https://github.com/wowchemy/starter-hugo-academic)
- [How to Create an Academic GitHub Page With Hugo?](https://mickaellalande.github.io/post/tutorial/how-to-create-an-academic-github-page-with-hugo/)