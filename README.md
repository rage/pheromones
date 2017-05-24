# pheromones

Pheromones is a Javascript-library that is used to track users' movements within a web page. It annotates each element within a web-page and tracks the elements that the user sees as she is browsing the web page. The library was developed as a part of a social navigation support class project by Tony Kovanen, Hanna Mäenpää and Arto Vihavainen quite a few years ago. Pheromones requires [Visibility.js](https://github.com/ai/visibilityjs) which makes it straightforward to determine whether the web page is visible to a user.

For Pheromones to work, you'll need a backend which can store (any) data.


```javascript
var user = "MY USER NAME FROM e.g. LOGIN MODAL";
var backend = "BACKEND ADDRESS TO WHICH PHEROMONES WILL PUSH DATA";
var submitInterval = 20; // "ticks between submitting data" -- tick length configured in Pheromones

pheromones.init({
    apiUrl: backend,
    username: user,
    submitAfter: submitInterval
});

```
