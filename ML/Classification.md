Classification is a supervised machine learning technique used to predict labels or categories based on input data. The goal is to assign each data point to a predefined class.

![[{C6805EBB-016E-4BE5-8030-5BECCE679C5A}.png]]
## Types of Classification

The process of sorting data into categories based on specific features or characteristics. There are different types of classification problems depending on how many categories (or classes) we are working with and how they are organized.

#### 1. Binary Classification
This is the simplest kind of classification. The goal is to sort the data into two distinct categories. Imagine a system that sorts emails into either spam or not spam. It works by looking at different features of the email like certain keywords or sender details and decides whether it’s spam or not.

#### 2. Multiclass Classification
The data needs to be sorted into more than two categories. The model picks the one that best matches the input. Think of an image recognition system that sorts pictures of animals into categories like cat, dog and bird.


![[{60F4D921-037E-4624-8CEC-96E1F1A97206}.png]]

#### 3. Multi-Label Classification
Single piece of data can belong to multiple categories at once. Unlike multiclass classification where each data point belongs to only one class, multi-label classification allows datapoints to belong to multiple classes. A movie recommendation system could tag a movie as both action and comedy. The system checks various features (like movie plot, actors or genre tags) and assigns multiple labels to a single piece of data, rather than just one.