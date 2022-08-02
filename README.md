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


