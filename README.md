# modestiq-docker

## Make backup of db database
`docker-compose exec -e 'MYSQL_PWD=root' db mysqldump -u root mydb > ./mysql/dump/backup.sql`
