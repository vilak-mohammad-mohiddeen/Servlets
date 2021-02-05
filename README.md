# Servlets
- tomcat
  - webapps
    - Application name
      - .html files
      - WEB-INF
        - classes
          - Servlets.java
        - web.xml
        - lib
          - mysql-connector.jar
# Servlet file
- inorder to make .java file to servlet we need to extend HttpServlet class by which our .java file becomes a servlet
- By extending we get 3 methods
  - public class MyServlet extends HttpServlet {<br>
    public void service(){<br>

    }<br>
    public void doPost(){<br>

    }<br>
    public void doGet(){<br>
        
    }<br>
}<br>
### Servlet gets request and sends response by 2 Objects
- HttpServletRequest req,HttpServletResponse res
<br> public void service(HttpServletRequest req,HttpServletResponse res){
<br> **getting parameters from client so req object will have access**
<br>req.getParameter('uname');
<br>}
- **generally, method="get" will show the parameters in url**
- **if method is not specified then its get method**
- **if method="post" it wont show parameters in url**
