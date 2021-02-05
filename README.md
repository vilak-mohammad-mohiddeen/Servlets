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
# public void service() will work for both get,post methods inorder to restrict we use doGet() and doPost() methods
- these work for there specific methods
# RequestDispatcher :: calls Servlet from a servlet
<br>RequestDispatcher rd=req.getRequestDispatcher("ser2");
<br>rd.forward(req,res);
- this request dispatcher does not tell browser whether response is given by ser1 or ser2
# sendRedirect :: it will tell browser which is sending response
res.sendRedirect("ser2");
