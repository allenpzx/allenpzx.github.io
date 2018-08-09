---
title: swiper by origin JavaScript
date: {{ date }}
tags:
- swiper
- CSS

---
## Swiper



#### Container component

```html
              <div className='swiper-view'>
                  
                  <div className='swiper-view-container'>
                      
                      <div className='swiper-view-item'>
                          ......
                      </div>

                      <div className='swiper-view-item'>
                          ......
                      </div>

                      <div className='swiper-view-item'>
                          ......
                      </div>

                  </div>
                  {/* swiper_view_content结尾处 */}
              </div> 
              {/* swiper_view整体容器结尾处 */}
```
<!-- more --> 


#### style

```scss
.swiper-view
    position: relative
    width: 100vw
    min-height: 30vh
    overflow: hidden

.swiper-view-container
    padding-bottom: 10px
    // height: 100%
    position: relative
    white-space:nowarp
    box-sizing: content-box
    display: flex
    flex-direction: row
    transition: transform 0.35s cubic-bezier(0.15, 0.3, 0.25, 1) 0s
    direction: ltr
    will-change: transform
    transform: translateX(0%)

    .swiper-view-item
        width: 100%
        height: 100%
        flex-shrink: 0
        // overflow: auto
        display: flex
        flex-direction: row
        flex-wrap: wrap
        justify-content: space-evenly
        align-items: flex-start
        position: relative
```

