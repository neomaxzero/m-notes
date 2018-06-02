## Suspense - Andrew Clark

https://www.youtube.com/watch?v=z-6JC0_cOns

### Optimizing the initial page load.

* Initial load time is critical

- Modern web apps require lots of stuff

  * JS
  * Data
  * Images.

- #1: Load less stuff.
- #2: Defer non-critical resources.
- #3: Code splitting.

- #4: Avoiding serial network requests.

- #5: Avoid innecesary placeholders.

- #6 Framework helpers: Don't fallback to placeholders immediately

### Requirements for the proposed solution:

* Prioritize important content.
* Defer Secondary content.
* Avoid accidental placeholders.
* Encapsulate data using components.

### Introduction React Suspense

* Start rendering even before the data has loaded.
* Pause any component until its data is ready.
* On a fast network, delay DOM mutation until the entire tree is complete.
* On a slow network, precisely control loading states.

### Server-side rendering

* Reduced latency between FE server and data sources.
* Can start displaying content before any JS has loaded.

Problems with SSR with React (no Next.js):

* Can't start rendering anything until everything has load.
* Need to hoist all async fetches.
* Encapsulation is difficult.

### Great Example (Check video)
