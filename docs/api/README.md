---
id: api-reference
title: API Reference
---

# API Reference

The Redux API surface is tiny. Redux defines a set of contracts for you to implement (such as [reducers](../understanding/thinking-in-redux/Glossary.md#reducer)) and provides a few helper functions to tie these contracts together.

This section documents the complete Redux API. Keep in mind that Redux is only concerned with managing the state. In a real app, you'll also want to use UI bindings like [react-redux](https://github.com/gaearon/react-redux).

### Top-Level Exports

- [createStore(reducer, [preloadedState], [enhancer])](createStore.md)
- [combineReducers(reducers)](combineReducers.md)
- [applyMiddleware(...middlewares)](applyMiddleware.md)
- [bindActionCreators(actionCreators, dispatch)](bindActionCreators.md)
- [compose(...functions)](compose.md)

### Store API

- [Store](Store.md)
  - [getState()](Store.md#getState)
  - [dispatch(action)](Store.md#dispatchaction)
  - [subscribe(listener)](Store.md#subscribelistener)
  - [replaceReducer(nextReducer)](Store.md#replacereducernextreducer)

### Importing

Every function described above is a top-level export. You can import any of them like this:

#### ES6

```js
import { createStore } from 'redux'
```

#### ES5 (CommonJS)

```js
var createStore = require('redux').createStore
```

#### ES5 (UMD build)

```js
var createStore = Redux.createStore
```
