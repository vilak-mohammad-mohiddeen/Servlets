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
