Next.js
It is a full stack React.js framework for building web apps.
In addtion to building UI components, it also provides features like routing, styling, data fetching, rendering, optimization, etc.
It uses react server component
It is opinionated framework (file, folder convention)
Features
Routing: file based routing
Rendering: Client side rendering (CSR), Server side rendering (SSR), Static site generation (SSG)
Optimization: images, fonts, scripts
Data fetching: Async data fetching
API routes
Styling
Routing
file based routing
All routes must be inside src/app directory
Every routes must have page.js or page.tsx
page.js or page.tsx file must have a default export react component
Simple routes
Create a folder inside src/app directory and add page.js file
/src/app/about/page.js
/src/app/products/page.js
Nested routes
/src/app/courses/backend/nodejs/page.js
/src/app/courses/backend/laravel/page.js
/src/app/courses/frontend/react/page.js
/src/app/courses/frontend/vue/page.js
Dynamic routes
Create a folder enclosed by [].
/src/app/products/[id]/page.js
Nested dynamic routes
/src/app/products/[id]/reviews/[reviewId]/page.js
Catch all segments
Create a folder enclosed by []
The route name should have rest operator as prefix
/src/app/blogs/[...slug]/page.js
Private folders
/src/app/_myfolder
Route groups
/src/app/(auth)/login
/src/app/(auth)/register