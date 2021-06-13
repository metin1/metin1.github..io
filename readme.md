
# Welcome My Github Page

My name is Metin İŞCAN, I am Full Stack Developer and I have 3+ years experince,
> Updated at 13 July 2021

###React
I had work with MERN (MongoDb, ExpressJs, React and NodeJS). I like to use React functional componenets and React Hooks.
###Next.Js
Also I always look for the future of the development skills. Because of the I had started my second project with [Next.Js](https://github.com/vercel/next.js,"Vercel "). I speed up my coding with Next.Js and I like to write over it.

** [Next.Js](https://github.com/vercel/next.js,"Vercel ") is React Framework for Production and gives developers the best developer experience with all the features developers need for production: hybrid static & server rendering, TypeScript support, smart bundling, route pre-fetching, and more. No config needed.**  [Official Site](https://nextjs.org/ ,"Vercel NextJs")

### Redux and SWR
I had code with Redux. I used every part of my first project. It simplified to control state that big project. Also I used SWR at my second project. [SWR](https://swr.vercel.app) is React Hooks library for data fetching and it is Fast, lightweight and reusable data fetching, has built-in cache and request deduplication. It offers me lots of things. Like, refrest fetching data with an interval and when user focused the page. I can easily sancronise page, auhentication, and I reduce my redux usage.

You can fetch the user data with a simple hook:
```javascript
export function useCurrentUser() {
  const { data, error, mutate } = useSWR("/api/user");
  const user = data?.user;
  return [user, { mutate }, { isLoading: !error && !data }];
}
```
You can manipulate your local data programmatically while updating at the back-end, while revalidating and finally replace it with the latest data.

```javascript
mutate('/api/user', { ...data, name: newName }, false)
// send a request to the API to update the source
await requestUpdateUsername(newName)
// trigger a revalidation (refetch) to make sure our local data is correct
mutate('/api/user')
```

### CSS and SVG
I like to optimise my code and search for pure css. Because pure css more secure and speedy. I used some simple svg instead of chart frameworks. I can easily send calculated date to svg and reshape it as I wanted with a few lines of codes.

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
