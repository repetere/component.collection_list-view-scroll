#Index

**Classes**

* [class: listViewScroll](#listViewScroll)
  * [new listViewScroll()](#new_listViewScroll)
  * [listViewScroll~defaults](#listViewScroll..defaults)
  * [listViewScroll.initEventListeners()](#listViewScroll#initEventListeners)
  * [listViewScroll.init()](#listViewScroll#init)
  * [listViewScroll._getViewportH()](#listViewScroll#_getViewportH)
  * [listViewScroll._scrollY()](#listViewScroll#_scrollY)
  * [listViewScroll._getOffset(el)](#listViewScroll#_getOffset)
  * [listViewScroll._scrollPage()](#listViewScroll#_scrollPage)

**Events**

* [event: "touchStartHandler"](#event_touchStartHandler)

**Members**

* [options](#options)
 
<a name="listViewScroll"></a>
#class: listViewScroll
**Members**

* [class: listViewScroll](#listViewScroll)
  * [new listViewScroll()](#new_listViewScroll)
  * [listViewScroll~defaults](#listViewScroll..defaults)
  * [listViewScroll.initEventListeners()](#listViewScroll#initEventListeners)
  * [listViewScroll.init()](#listViewScroll#init)
  * [listViewScroll._getViewportH()](#listViewScroll#_getViewportH)
  * [listViewScroll._scrollY()](#listViewScroll#_scrollY)
  * [listViewScroll._getOffset(el)](#listViewScroll#_getOffset)
  * [listViewScroll._scrollPage()](#listViewScroll#_scrollPage)

<a name="new_listViewScroll"></a>
##new listViewScroll()
A module that represents a listViewScroll object, a List view collection page.

**Author**: Yaw Joseph Etse  
**License**: MIT  
**Copyright**: Copyright (c) 2014 Typesettin. All rights reserved.  
<a name="listViewScroll..defaults"></a>
##listViewScroll~defaults
module default configuration

**Scope**: inner member of [listViewScroll](#listViewScroll)  
<a name="listViewScroll#initEventListeners"></a>
##listViewScroll.initEventListeners()
Sets up a new listViewScroll event listeners.

<a name="listViewScroll#init"></a>
##listViewScroll.init()
Sets up a new listViewScroll component.

<a name="listViewScroll#_getViewportH"></a>
##listViewScroll._getViewportH()
handle touch start events

**Returns**: `number` - height of viewport element  
<a name="listViewScroll#_scrollY"></a>
##listViewScroll._scrollY()
get the scroll position of the viewport element

<a name="listViewScroll#_getOffset"></a>
##listViewScroll._getOffset(el)
get element offset, http://stackoverflow.com/a/5598797/989439

**Params**

- el `object` - element of scrolled element  

**Returns**: `object` - top,left position of element  
<a name="listViewScroll#_scrollPage"></a>
##listViewScroll._scrollPage()
Keep visible sections in viewport

<a name="event_touchStartHandler"></a>
#event: "touchStartHandler"
handle touch start events

**Params**

- el `object` - element to check if in viewport  
- h `object` - element to check if in viewport  

<a name="options"></a>
#options
extended default options

