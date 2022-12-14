# OVERVIEW
## the-concept-of-composition
### Contents
* Composistion using children prop; Card component has a common style and wrap Card around other components to render the common style 

## portals
### Contents
* Use of portal for displaying Error Modal
* use of Wrapper (vs. Fragment)

<img width="647" alt="portals-1" src="https://user-images.githubusercontent.com/29666846/208266894-94b824d2-5dca-450d-a285-0d30016f5208.png">

## ForwardRef ReactContext UseReducer UseState UseEffectCleanUp

### LESSONS LEARNED
* setTimeout debouncer with useEffect hook w/ cleanup function
* Use of Forward Ref for <Input /> using useImperativeHandle
* useContext for global "auth" state
* useReducer for complex state dependency

## Error Boundary

### LESSONS LEARNED
* Error Boundary needs to be in Class Components


## Custom Hook

### LESSONS LEARNED
* placeholder

## Form UseReducer

### LESSONS LEARNED
* various ways to create the form input using useReducer & custom hook

![image](https://user-images.githubusercontent.com/29666846/208586212-06822000-7e39-4c4a-acb2-abfff6b452af.png)

## Redux Toolkit

### LESSONS LEARNED
* reduxToolkit uses immer
* redux-toolkit includes redux; therefore, it's safe to delete redux library
* React Context has a bad performance; React context is ready to be used for low frequency unlikely updates (like locale/theme); not ready to be used as a replacement for all Flux-like state propagation
* Q: what's the use case of mix-match Redux and React Context

## Redux Thunk

### LESSONS LEARNED
* side-effects and async tasks can be executed 1) inside the component (e.g., useEffect()) 2) inside the action creators
* Redux Thunk pattern : dispatch wrap around dispatch

---


# LESSONS LEARNED

## [setup] 1. remove the folder from submodule

If all you want is to put your submodule code into the main repository, you just need to remove the submodule and re-add the files into the main repo[stack overflow](https://stackoverflow.com/questions/1759587/how-to-un-submodule-a-git-submodule)
```
git rm --cached submodule_path # delete reference to submodule HEAD (no trailing slash)
git rm .gitmodules             # if you have more than one submodules,
                               # you need to edit this file instead of deleting!
rm -rf [-r -fo] submodule_path/.git     # make sure you have backup!!
git add submodule_path         # will add files instead of commit reference
git commit -m "remove submodule"
```

TODO: Terminal Command - check the difference between `rm -rf` vs. `rm -r -fo`

---
