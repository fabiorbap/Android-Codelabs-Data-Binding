## Android-Codelabs-Data-Binding
Repository with the Data Binding Codelabs exercises

Base code obtained in https://github.com/googlecodelabs/android-databinding

------------
What I learned:

- Using too many findViewById is expensive and can make the app slower, because the app traverses the view hierarchy starting at the root until the required view. This information matches with the advantage of the Constraint Layout having a more flat view hierarchy, which improves performance.
- findViewById is checked in runtime, which means the app can crash if the id doesn't exist, making it a dangerous approach to locating view ids
- The layout variables declared in the <data> tag in the XML are used in layout expressions, which are placed in the value of element attributes. It is not a good idea to write complex logic into these layout expressions, which can make the layout complicated to read and to maintain
- Some of the advantages of using databinding are: 1) Easier to maintain code and reduction of code logic in activities and fragments 2) Performance improvements 3) Help prevent NPE and memory leaks
