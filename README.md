## Event Loop Assignment
# Answers to Numbers 1-5

1. The Event loop allows for asynchronous programming by handling events and callbacks. It also allows for non-blocking asynchronous I/O operations. When an event is triggered, its associated callback function is added to the event queue, and the event loop processes the queue one event at a time, executing the associated callback function for each event.
2. 
* Timers Phase: This phase is where callbacks scheduled by setTimeout(), setInterval() and setImmediate() whose time has expired, are executed.
* Pending Phase: This phase is where I/O related callbacks such as network requests and file system operations are executed.
* Idle, Prepare phase: These phases are internal phases of the event loop and are used to optimize its performance.
* Poll Phase: In this phase, the event loop waits for new I/O events and executes callbacks related to completed I/O operations. If there are no I/O events, it will move on to the check phase. 
* Check phase: This phase is where setImmediate timers as part of the I/O in the Poll phase are executed.
* Close Callback Phase: This is where close event callbacks are executed. If there are no Timers or I/O calls left, the event loop closes and the process ends. 

3. 
- Focus on code quality.
- Prefer ES6+ and Async/Await
- Keep code small
- Handle errors

4. NPM5 is a version of NPM (Node Package Manager) that introduced several new features and improvements, such as a new package-lock.json file for deterministic dependency resolution and improved performance.
To initialize a package in NPM, you can use the following command in the terminal: 
npm init

5. To run a script in the package.json file, you use the "npm run" command followed by the name of the script. 
For instance, if there is a script named "start" in your package.json file, you can run it using the following command on the terminal:
npm run start
