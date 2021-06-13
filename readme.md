
# Welcome My Github Page
> Updated at 13 July 2021

My name is Metin İŞCAN, I am full stack developer and, I have 3+ years experience,

### React
I had worked with MERN (MongoDB, ExpressJs, React and NodeJS). I like to use functional components of React and React Hooks.
### Next.Js
Also, I am always looking for the future of development skills. For this reason, I started my second project with [Next.Js] (https://github.com/vercel/next.js, "Vercel "). I'm accelerating my coding with Next.Js and love writing with it.

** [Next.Js](https://github.com/vercel/next.js,"Vercel ") is React Framework for Production and gives developers the best developer experience with all the features developers need for production: hybrid static & server rendering, TypeScript support, smart bundling, route pre-fetching, and more. No configuration needs.**  [Official Site](https://nextjs.org/ ,"Vercel NextJs")

### Redux and SWR
I had code with Redux. I used every part of my first project. It made it easier to control the state of this big project. For my second project, I also used SWR. [SWR] (https://swr.vercel.app) is React Hooks library for data queries and it is fast, lightweight, reusable, has built-in cache and deduplication of queries. It provides a wide range of functions. For example, refreshing the data at a specific interval and when the user focuses the page. I can easily synchronize the page, authentication, and I reduce my redux usage.

I can fetch the user data with a simple hook:
```javascript
export function useCurrentUser() {
  const { data, error, mutate } = useSWR("/api/user");
  const user = data?.user;
  return [user, { mutate }, { isLoading: !error && !data }];
}
```
I can programmatically manipulate my local data as I update, revalidate, and eventually replace it with the latest data on the backend.

```javascript
mutate('/api/user', { ...data, name: newName }, false)
// send a request to the API to update the source
await requestUpdateUsername(newName)
// trigger a revalidation (refetch) to make sure our local data is correct
mutate('/api/user')
```

### CSS and SVG
I like to optimise my code and pay attention to pure css. Because pure css is more secure and faster. I use a simple svg instead of chart frameworks. I can just send calculated data to svg and transform it the way I want with a few lines of code.

This is simple code of line chart with svg:
```javascript
`<svg
	className="mx-3"
	width={72}
	height={170}
	viewBox="0 0 72 170"
	fill="none">
	<defs>
	  <linearGradient
		id={"pro" + i}
		x1={0}
		y1={1}
		x2={0}
		y2={0}>
		<stop
		  id={"a" + i}
		  offset={
			parseInt(monthLesson) > weeklyObj * 4
			  ? 1
			  : parseInt(monthLesson) / (4 * weeklyObj)
		  }
		  stopColor={
			i !== 2
			  ? "var(--text-hint)"
			  : "var(--primary-color)"
		  }
		/>
		<stop
		  id={"b" + i}
		  offset={
			parseInt(monthLesson) > weeklyObj * 4
			  ? 1
			  : parseInt(monthLesson) / (4 * weeklyObj)
		  }
		  stopColor="#FFF4F4"
		/>
	  </linearGradient>
	</defs>
	<path
	  id="my-shape"
	  d="M4 0.5H67.86C69.793 0.5 71.36 2.067 71.36 4V169.5H0.5V4C0.5 2.067 2.067 0.5 4 0.5Z"
	  fill={`url(#${"pro" + i})`}
	  stroke="#757575"
	/>
</svg>`
```
