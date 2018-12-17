
Spring Boot soap webservice 示例

wsdl 地址
```
http://localhost:8080/ws/countries.wsdl
```

测试方法 
postman
POST  
text/xml

url 
```
http://localhost:8080/ws
```

xml如下
```xml
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
				  xmlns:gs="http://spring.io/guides/gs-producing-web-service">
   <soapenv:Header/>
   <soapenv:Body>
      <gs:getCountryRequest>
         <gs:name>Spain</gs:name>
      </gs:getCountryRequest>
   </soapenv:Body>
</soapenv:Envelope>
```

-----

SoapWsClient是Spring boot client代码

---

都是官方示例

链接

https://spring.io/guides/gs/producing-web-service/
https://spring.io/guides/gs/consuming-web-service/