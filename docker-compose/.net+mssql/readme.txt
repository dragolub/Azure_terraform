0. Open project by Visual Studio
1. Create docker files - from Visual Studio -> docker support
2. Move docker files to *.sln files
3. Build docker - docker build -t nameapp .
4. docker run -p 80:80 nameapp
5. Check SQL server appsettings.json - name and pass from SQL
6. docker create volume sqldata
7. create docker-compose file 
8. docker-compose -f 'path-name 'build | up -d | down
9.1. login in Azure - az login
9.2. az group create --name dragolub*****rg --location westeurope  ------ create container regesty 
10. az acr create --resource-group dragolub*****rg --name dragolub*****cr --sku Basic ----- create container registry into registry
11. rename docker image - docker tag my_app dragolub*****cr.azurecr.io/myapp 
12. Add image in docker-compose file
13. push image in az container regesty 
13.1. az acr login --name dragolub*****cr.azurecr.io/myapp 
13.2. docker push dragolub*****cr.azurecr.io/myapp 
14. docker context create aci my_appcontext
15. docker context use my_appcontext
16. docker-compouse up -d  -2:00:00 lekciqta