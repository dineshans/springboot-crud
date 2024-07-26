# springboot-crud

# Maven build command 
1) mvn clean install
2) mvn clean install -DskipTests

# Rest API end Point - curl command

1) GET API:
		curl --location 'localhost:8080/api/employees/empDetails'

2) POST API: 

		curl --location 'localhost:8080/api/employees/createEmployees' \
		--header 'Content-Type: application/json' \
		--data '{
			"name": "Dinesh Sahu",
			"role": "Developer"
		}'
		
3) Update API:

		curl --location --request PUT 'localhost:8080/api/employees/updateEmployee?id=1' \
		--header 'Content-Type: application/json' \
		--data '{
			"name": "Dinesh",
			"role": "Developer & DevOps"
		}'