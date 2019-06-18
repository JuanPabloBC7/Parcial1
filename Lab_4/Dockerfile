FROM node:8

# Create app directory
WORKDIR /usr/src/app

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

EXPOSE 3000
#CMD ["mysql -h localhost -u root -p Juanpablo7$"]
#CMD ["CREATE DATABASE jpbalan;"]
#CMD ["USE jpbalan;"]
#CMD [" CREATE TABLE Productos(
#			ID_Producto INT(5) NOT AUTO_INCREMENT,
#			Nombre VARCHAR(200),
#			Precio INT(11)
#			CONSTRAINT ProductoPK PRIMARY KEY (ID_Producto)
#		)ENGINE INNODB;"]
#CMD ["SHOW TABLES"]
#CMD ["QUIT"]
CMD [ "node","src/app.js" ]