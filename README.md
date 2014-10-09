XmiParser
=========

XmiParser is XMI Model parsing framework for validation and HTML
javadoc generation. Given XMI XML input file it creates simple
structures to enable subclasses to quickly validate, generate
HTML from the model or convert to other forms.

Parser will iterate over each element and package in the model.

The HTML generator generates javadoc-like HTML documentation
with javadoc summary pages and detailed class-level pages.

If a class or interface inherits from multiple super classes or interfaces then
multiple views will be created. The default view will list all the attributes
grouped by the class that it inherits those from. The second view will be
a flat sorted list of attributes with hyper links back to the parent classes
or interfaces that they are inherited from.

HTML generator also creates two summary files that list all the classes
and packages of the model (e.g. xxx.xmi-list.txt) as well as a detailed
listing of all attributes for each class or interface (e.g. xxx.xmi-details.txt).

Note that Enterprise Architect can export EAP models as XMI 1.1 or 2.1.
XMI file must be version 2.1 and UML must be 2.1 or 2.2. Other versions
are not supported by the parser.

# License

Copyright 2014 The MITRE Corporation

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.