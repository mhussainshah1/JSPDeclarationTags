JSP Tags
--------

1) **JSP Expression Tag** - allow us to directly put Java expressions into an HTML file. This includes math expressions,
   boolean expressions, and calling methods that return values to be displayed on the page.

- Calling a method: `<%= Math.addExact(2, 3) %>`<br>
  ` <%= add(34, 5)%> `<br>
  `<%= subtract(56, 18)%>`


- Evaluating a boolean: `<%= "bob".length() < 3 %>`
- Math Expression: `<%= (500.6 * 7) - 50 %>`
- Java Object: `<%= LocalDateTime.now() %>`

In each of the examples, they are implicitly being converted into Strings before being added to Html

2) **JSP Scriptlet Tag** - use to only define variable

<pre>
    <%
        int bob = 150;
    %>
</pre>

3) **JSP Comment** - used to define comments

   `<%-- This is how you make a JSP comment --%>`

   `<!-- HTML comments are also valid in jsp file -->`


4) **JSP Declaration** - used to define variables and methods

<pre>
    <%!
        int bob = 150;

        int add(int num1, int num2) {
            return num1 + num2;
        }

        int subtract(int num1, int num2) {
            return num1 - num2;
        }
    %>
</pre>



