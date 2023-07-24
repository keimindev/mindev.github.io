---
layout: post
title:  "[React] SSR vs CSR"
author: min
categories: [blog, react, next.js, study, frontEnd]
tags: [리액트, react, 테크공부, nextjs, csr, ssr]
image: https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2F4C1Or%2FbtsoRDM4RC5%2F0OoR9iLfZJTJ3V9ZH4jULk%2Fimg.jpg
featured: true
---
<br>

## What's difference between SSR and CSR?

### CSR (Client-Side Rendering) 
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FmvAPF%2FbtrcM1fGQEJ%2FoqGeGnUFg9wXZOkClMC39k%2Fimg.png" alt="csr"/>
<p>In CSR, the initial HTML page is loaded with minimal content and often includes JavaScript files. The client-side JavaScript then takes over and fetches data from the server and renders the rest of the page dynamically. This approach provides a more interactive user experience because the user can see and interact with the page while the data is being loaded and rendered. Popular JavaScript frameworks like React, Angular, and Vue.js are commonly used for CSR.</p>
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbkJ0my%2FbtrcOM9GT1V%2FaKDCRhm77MfHF8ushplGi0%2Fimg.png" alt="csr2" />
<br>

##### Advantages of CSR
- Fast initial page load as the server sends minimal content. 
- Enhanced user experience due to dynamic rendering and interactivity. 
- Better support for single-page applications (SPAs) and complex user interfaces.

##### Disadvantages of CSR
- Potentially slower data loading as the client needs to fetch data after the initial page load.
- Poor SEO (Search Engine Optimization) unless additional measures like server-side rendering or pre-rendering are implemented.
- Increased client-side processing, which may lead to slower performance on low-end devices.


<br>
<br>

### SSR (Sever-Side Rendering)
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2F6J4Fs%2FbtrcNnv3HWf%2F3f3KnWPKUBtlU7HshmcuOK%2Fimg.png" alt="ssr" />
<p>In SSR, the web server processes the client's request and generates a fully rendered HTML page on the server-side. The complete page with all its content is then sent to the client, which can be displayed instantly. SSR is particularly useful for content-heavy websites or when SEO is a priority, as search engines can index the fully rendered content.</p>

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FdGCZHY%2FbtrcOfdcohI%2FDKF2Cr2HHW5X8vNSaexEpK%2Fimg.png" alt="ssr2" />
<br>

##### Advantages of SSR
- Faster time to first paint and content display since the server sends a fully rendered page.
- Improved SEO, as search engines can easily crawl and index the content.

##### Disadvantages of SSR
- Potentially slower initial page load, especially for complex pages with a lot of data to fetch.
- Reduced interactivity until the client-side JavaScript takes control.
- Higher server load compared to CSR, as the server has to handle rendering for each request.

<br>
<br>

In summary, CSR is preferred for applications that require high interactivity and frequent updates after the initial page load. SSR is beneficial for content-heavy websites or when SEO is a priority. In some cases, developers use a hybrid approach, where they leverage the advantages of both CSR and SSR based on specific requirements and use cases.


<br>
<br>
