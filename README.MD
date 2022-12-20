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
