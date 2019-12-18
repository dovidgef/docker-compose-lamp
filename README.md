# modestiq-docker

## Make backup of db database
`docker-compose exec -e 'MYSQL_PWD=root' db mysqldump -u root mydb > ./mysql/dump/backup.sql`

# Restore
`cat backup.sql | docker-compose exec -e 'MYSQL_PWD=root' db mysql -u root mydb`
