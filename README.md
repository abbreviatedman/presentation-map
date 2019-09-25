# The Marpit Slideshow Template Repo


This is a template repo with all the code to turn a marpit markdown file into a slideshow presentation that can be served live or made into an online version.


### Setup

1. Copy this repo.
2. Place a `PITCHME.md` file using [Marpit's markdown style](https://marpit.marp.app/markdown) in the root level. 
3. 
```bash
npm install
```
4. Consider updating this README for your new presentation!


### To Serve Live Locally

```bash
npm run start
```


### To Build for Deployment

```bash
npm run build
```


### To Deploy As Webpage Using Surge

Install `surge` if necessary:
```bash
npm install -g surge
```
After building for deployment:
```bash
cd dist
surge
```