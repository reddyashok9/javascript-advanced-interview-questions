# javascript-advanced-interview-questions

# 1. Why Promises Are Faster Than setTimeout()?

Promise.resolve(1).then(function resolve() {
  console.log('Resolved!');
});
setTimeout(function timeout() {
  console.log('Timed out!');
}, 0);
// logs 'Resolved!'
// logs 'Timed out!'

Because of the event loop priorities dequeuing jobs from the job queue (which stores the fulfilled promises' callbacks) over the tasks from the task queue (which stores timed out setTimeout() callbacks).



