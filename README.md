provider "aws" {
    region = "us-east-1"
  
}
resource"aws_instance" "webserver" {
    ami="ami-0cbbe2c6a1bb2ad63"
    instance_type ="t3.micro"
     tags={
        Name ="Apache webserver"
    }

}
