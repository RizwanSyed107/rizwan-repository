// Firewall Discovery Service
Environment used:
-----------------------
	1. Apache Tomcat Container (apache-tomcat-8.5.47)
	2. Java 1.8
	3. Mysql Database

Deployment Steps:
--------------------------
1. Update 'routeinfo.properties' with Database connection information.
2. Run the SQL script with name 'routeinfo_schema.sql'. This will create schema and necessary tables.
3. Run 'parse_store_res.bat' which will invoke the parser and storage handler that processes the resource XML files present in folder 'route_xml_res'.
4. Deploy the war file 'fds.war' to Tomcat webapps directory.
5. Place a copy of 'routeinfo.properties' in Tomcat bin directory (apache-tomcat-8.5.47/bin).
6. Start Tomcat container
7. Open browser and put service URL
	http://localhost:8080/fds/ui/   (OR)   http://localhost:8080/fds/ui/index.html
				
