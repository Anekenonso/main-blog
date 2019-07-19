---
title: I made a little change 
date: "2019-07-19"
---

I made a little change to some part of the codes, so this content is just a dummy text

The problem turned out to be incredibly simple.

```javaScript
()=>{
      console.log("still a dummy text");
}

();
```


My Gatsby site has been live on Netlify for over a year now. The entire time I've had an environment variable set in the Netlify UI for ENV=production. Originally added that to make CSS compile and link correctly on the live site.

So, what was happening is my devDependencies were not installing at build time on Netlify. Resulting in unclear errors.

The Fix
Changed to ENV=development and the build process went through like a charm.

Still need to test the live site thoroughly, but I believe the problem is solved!