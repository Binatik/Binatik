# Serega Mangushev  
Junior WEB developer, Russia.

[TOCM]

# Skills 
### Imposer 

Layout of simple / medium-sized sites for more than a year. Easy work with javaScript for less than a year. 
Bootstrap framework and Sass preprocessor.
 
### Front-end logic 

Working with javaScript. Learning the REACT framework and VUE.

### SSR/SPA   
 
Experience working with react in conjunction with the next framework on react for 
Server Side Rendering 

typeScript skills.

# Other skill   

Knowledge of photoshop, the git system in particular gitHub Desktop.  

Simple skills when working with python.  

Experience in developing gulp, in particular webpack.  

# Code 
 
//This code was written in this editor by hand.  

```js
function getArr(...arg){
    return arg.map(element => element+element)
} 

```   

```js
const posts = [

    {
        id: 1,
        author: 'Binatik',
        text: 'This id will not show the function, because the property is an empty string.',
        photos: '',
    },

    {
        id: 2,
        author: 'Binatik',
        test: 'This id will be shown by the function.',
        photos: '/url/photos',
    },

]

function getPosts(arr){
    return arr.filter(({ photos }) => (photos.length !== 0));
}

getPosts(posts)

```     

```js 
/* 
Note: This code is a separate class that cannot function without an additional class.  
It needs to accept the modal window itself.
*/ 
 
class Popup {
    constructor(popup) {
        this.popup = popup;
        this.popup.addEventListener('click', (event) => this.modalClose(event));
    }

    modalOpen(){
        this.popup.classList.add('modal-open');
    };

    modalClose(e){
        const target = e.target;
        if (target.classList.contains('modal')){
            target.classList.remove('modal-open');
        }

        if (target.classList.contains('p-info__btn-close')){
            this.popup.classList.remove('modal-open');
        }
    };
}
```  









