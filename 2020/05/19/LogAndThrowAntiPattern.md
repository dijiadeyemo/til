# Log And Throw AntiPattern

**Author** : Diji

## Notes

This is usually not a good idea because the upstream handler of the error should be the one deciding whether it should be logged or not.

### Exception
* Is there valuable information here that should be logged but may be lost in the upstream handler? In this case, it may be okay to log and throw.
