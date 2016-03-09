# Resources

This pge documents a few resources on the website.

## Diagram

The diagram is created using [yED](https://www.yworks.com/products/yed).


## Client Tag Cloud

The Client cloud on the home page is created the following way:

Generated on this site: http://timdream.org/wordcloud2.js

Word list:

```
6 Guzzle
6 cURL
6 Socket
5 Buzz
5 Zend
4 HTTPful
5 React
3 file_get_contents();
4 Cake
4 PECL
4 Requests
```

Configuration:

``` json
{
  gridSize: Math.round(16 * $('#canvas').width() / 1024),
  weightFactor: function (size) {
    return Math.pow(size, 2.3) * $('#canvas').width() / 1024;
  },
  fontFamily: 'Impact',
  color: function (word, weight) {
    var items = ['#E6B74C', '#CE1A38', '#E2D27F', '#B4CC52', '#B4CC52', '#4D4D4D', '#E96F7F', '#27AAE2', '#02467A'];
    return items[Math.floor(Math.random()*items.length)];
  },
  rotateRatio: 0.5,
  backgroundColor: '#ffffff'
}
```

TODO: Might be a good idea to integrate the library itself:

https://github.com/timdream/wordcloud2.js
