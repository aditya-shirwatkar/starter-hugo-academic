# Academic Webpage

A repo for building [my website](https://aditya-shirwatkar.github.io) using Hugo and host it on github pages

## Dependencies for building

- [Hugo](https://gohugo.io/)
    - wget <extented deb name from>
    - sudo dpkg -i hugo_0.109.0_linux-amd64.deb
- [Go](https://go.dev/)

## Updating Commands

```bash
git add .
git commit -m "Making Changes"
git push -u origin main

hugo # Generate the website inside the public directory
cd public
git add .
git commit -m "Build website"
git push origin main
cd ..
```

## Useful Links

1. https://github.com/matteocourthoud/custom-wowchemy-theme/issues/1

## Credits

- [Hugo Academic Theme](https://github.com/wowchemy/starter-hugo-academic)
- [How to Create an Academic GitHub Page With Hugo?](https://mickaellalande.github.io/post/tutorial/how-to-create-an-academic-github-page-with-hugo/)