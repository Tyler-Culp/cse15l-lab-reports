Two of the tests that gave different results between the two markdown parsers were test 194 and test 201. In both of these tests my markdown parser returned nothing while the other parser returned one url in each test. The way I was able to quickly find tests that gave different inputs was by using vimdiff.

Here are the links to the two different test files:

* [Test 194](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md)
* [Test 201](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md)

For test 194 the correct implementation is my parser which returns no links. For test 201 I  think the other implementation,  which returns a link, is correct. Here are the two different outputs shown with vimdiff:

![SS1](LabReport5SS1.png)

I think that bug in my code causing the problem when we try test 201 is the fact that there is no real part addressing mulitline links that are created using colons. My markdown parser only just checks if there is a bracket pair and parenthesis pair set up such that the closed bracket is right next to the open paranethesis meaning htat it will never catch multi lined links. 

