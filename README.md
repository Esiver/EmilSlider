# EmilSlider
a simple slider by me

# to use, do something like this in your js:

import SlideBuilder from './EmilSlider.js'

let slideBuilder = new SlideBuilder();
let headerSlider = slideBuilder.buildSlide({
    containerSelector:"#header-slider",
    slidesListSelector: "#header-slider ul",
    slidesSelector:"#header-slider li",
    rightArrowSelector:"#header-slider-right",
    leftArrowSelector:"#header-slider-left"

});


# and something like this in your scss:

.slider {

    &__container {
        display: flex;
        overflow: hidden;
        

    }
    &__list {
        display: flex;
        flex-direction: row;
        gap: 10px;
        margin: 0;
        padding: 0;
        transition: transform 0.5s ease-in-out;
    }
    &__item {
        height: 100%;
        background-color: lime;
        margin: 0;
        min-width: 150px;
        
    }
    &__slide {
        width: 100%;
        height: auto;
        position: relative;
    }
}
