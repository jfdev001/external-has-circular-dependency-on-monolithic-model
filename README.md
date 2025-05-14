# External has Circular Dependency on Monolithic Model

In monolithic model cases, e.g., ICON, it is possible that 
a part of it that you would like to be factored into an external
library has a circular dependency on some core part of the monolithic
model's source code. Consider JSBACH and ART in ICON. These are both
integrated into the ICON build system, and thus are not true 
externals even though they are a compiled as such. The current
repository is for thinking about how one might handle extracting
a feature or set of features from a monolithic model to an external
library.
