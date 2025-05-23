# Unduck

DuckDuckGo's bang redirects are too slow. Add the following URL as a custom search engine to your browser. Enables all of DuckDuckGo's bangs to work, but much faster.

```
https://unduck.0xgingi.xyz?q=%s
```

## What does this Branch/Fork do different from vanilla unduck?

### Fork
 * Docker Support

### Branch
 * Docker Support
 * Add Kagi search engine & set it as default
 * Change T3.CHAT to use beta.t3.chat & Use Gemini-2.5-Pro with Search Enabled
 * Bun > PNPM


## How is it that much faster?

DuckDuckGo does their redirects server side. Their DNS is...not always great. Result is that it often takes ages.

I solved this by doing all of the work client side. Once you've went to https://unduck.link once, the JS is all cache'd and will never need to be downloaded again. Your device does the redirects, not me.