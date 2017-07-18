# Todo-List
Learning Redux
* Action represet "what happend" 
* Reducers update the state according to those actions
=> Store is the object that brings them together. It has responsibilities:
 -Holds application state
 -Access state via getState()
 -update state via dispatch(action)
 -Listener via subscribe(listener)
 -Handles unregistering of listeners via function return by subscribe(listener)
 
We'll only have a single store in Redux app. When want to split data handling logic, use reducer compostion instead of many stores.

Use combineReducers() to combine several reducers into one. 
We may optionally specify the initial state as second argument to createStore(). This useful for hydrating the state of the client to match the state of a Redux application running on sever
