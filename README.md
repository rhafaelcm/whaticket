https://www.youtube.com/watch?v=O1qGAkWM9-0

====================================

### EXECUTAR DOCKER DESKTOP
docker run --name comunidadezdg -e MYSQL_ROOT_PASSWORD=comunidadezdg -e MYSQL_DATABASE=whaticket-zdg -p 3306:3306 -d mysql

### WHATICKET
cd desktop
git clone https://github.com/pedroherpeto/whaticket.git

### ABRIR GIT CMD
cd Desktop
cd whaticket

### BACKEND
cd backend
npm install
npx sequelize db:migrate
npx sequelize db:seed:all
npm start

### FRONTEND
cd frontend
npm install --force
npm run build
npm start
