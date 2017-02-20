# Move SmartHome Designer to separate repository

To work on I created
* a "designer-removal" branch in my [Eclipse SmartHome repository fork](https://github.com/maggu2810/smarthome/tree/designer-removal)
* a new [repository "smarthome-designer" on my Github accout](https://github.com/maggu2810/smarthome-designer)

## Checklist: done

### smarthome

* Move all designer related stuff from `smarthome` to `smarthome-designer`
* Remove all entries / references in parent poms, features
* start test build with an empty local maven repository

### smarthome-designer

* Move all designer related stuff from `smarthome` to `smarthome-designer`
* Change the group ID in the poms to start with `org.eclipse.smarthome.designer` (so, add `designer` in the group ID between the smarthome part and the stuff after that / the end), all done except model.ui bundles
* TP: Copy the targetplatform from `smarthome` to `smarthome-designer`
* TP: use the `smarthome-designer` targetplatform
* TP: add the Eclipse SmartHome update-stable p2 repository
* `smarthome-designer`: start test build with an empty local maven repository

## Checklist: todo

### common

* What are the model.ui bundles used for (model.ui needs designer bundles) and who is using it at all (no feature found)?

### smarthome

* TP: Remove obsolete repositories

### smarthome-designer

* Remove unnecessary stuff in the POMs
* Remove unnecessary files
* TP: Remove obsolete repositories
