# zipkin
Tracing micro-services using Zipkin



**************** Zipkin demo **************

Step 1: start zipkins server first
			
			> java -jar zipkin-server-2.11.7-exec.jar
			
Step 2: Open browser and enter url to check if the zipkin server is up:
		
			http://localhost:9411/zipkin
			
# Now run the microservices registered to the zipkin server

step 3: Open project folder and build the project

			> mvn clean install
			
			Or Simply run "Build-all.bat" file.
		
		
Step 4: Now run each spring boot microservices 
		
			or run "Start-all.bat" file
			
			
Step 5: Open browser and go to the url "http://localhost:8081/zipkin"

		Note: There is an intentional delay in one of the services just to show in the trace.
		

Step 6: Now open zipkin dashboard (http://localhost:9411/zipkin) and click on "Find Traces" button.

		You will get the entire flow of the services registered in zipkin server.
		
