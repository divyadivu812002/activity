<%@page isELIgnored="false" %>

<%@taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>

<c:set var="var1" value="200"/>

<c:set var="var2" value="100"/>

<c:if test="${var1 > var2}">
	${var1} is greater the ${var2}
</c:if>
<br/>

<c:set var="color" value="RED"/>

<c:choose>
<c:when test="${color=='GREEN'}">
GREEN	

</c:when>	
<c:when test="${color=='RED'}">
RED	

</c:when>	
<c:when test="${color=='BLUE'}">
BLUE

</c:when>	


</c:choose>


<c:forEach var="num" begin="1" end="10">
	17 X ${num}=${17*num}<br/>

</c:forEach>


<c:forTokens var="fruits" 
items="Apple,Bannana,Mango,Strawberry,PineAppple" 
delims=",">
	${fruits}<br/>
</c:forTokens>
