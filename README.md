# PhotoZoom

Simple, lightweight jQuery plugin to show zoomed view of image based on screen dimensions. It simulates photo zoom for facebook (Chrome extension).

## The reason why I foked from [arunkumarsekar/photoZoom](https://github.com/arunkumarsekar/photoZoom)
- It is not maintained any more.
- It uses deprecated method `live`
- It has bug on represent bottom layer

## Browser Support

 - Internet Explorer 7+
 - Firefox
 - Chrome
 - Safari

## jQuery

	- Jquery Library (version 1.7.0+)

## How to use

### Init

```javascript
    $(document).ready(function(){
        $(selector).photoZoom();
    });
```
### Options

    - zoomStyle     // Write your own css for large image

#### Example

```javascript
     $(document).ready(function(){
         $("body").photoZoom({ zoomStyle : { "border":"1px solid #ccc",
                                             "background-color":"#fff",
                                             "box-shadow":"0 0 5px #888"
                                           }
                            });
     });
```

### Events

    - onMouserOver(currentImage)        // Triggers when before zooming image
    - onMouseOut(currentImage)          // Triggers when focus out from image

#### Example

```javascript
     $(document).ready(function(){
         $("body").photoZoom({ onMouseOver  : function(currentImage){
                                                console.log(currentImage);
                                                // do something
                                              },
                               onMouseOut   : function(currentImage){
                                                console.log(currentImage);
                                                // do something
                                              }
                            });
     });
```
## Demo

    - Demo : <http://yoonsy.github.io/photoZoom>
