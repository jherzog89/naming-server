<img width="844" height="379" alt="image" src="https://github.com/user-attachments/assets/30151098-6e65-46a0-b74d-e319165e31e8" />


docker run --name naming-registry-container --network my-app-network -p 8761:8761 jherzog89/naming-registry-service:v1
docker run --name authentication-container --network my-app-network -p 8777:8777 jherzog89/authentication-service:v1
docker run --name api-gateway-container --network my-app-network -p 8765:8765 jherzog89/api-gateway-service:v1
docker run --name reverse-string-container --network my-app-network -p 8080:8080 jherzog89/reverse-string-service:v1
