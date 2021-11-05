# mysqld_expoter 

将原始的版本改成支持多个实例的，多个实例用逗号“,”分隔


### Test
go test ./collector/ -v 
go test mysqld_exporter.go -v

### Build
go build -o mysqld_exporter mysqld_exporter.go 


### Running
export DATA_SOURCE_NAME='user1:password1@(127.0.0.1:3306)/,user2:password2@(127.0.0.1:3307)/'
./mysqld_exporter 

