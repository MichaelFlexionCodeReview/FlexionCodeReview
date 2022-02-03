# FlexionCodeReview
NB: All codes are merged to the master branch

# To host your Website on AWS EC2.
First  zip the folder for the web files.
Next log into the management console and select S3 under service.
Create a bucket and upload that zip folder into that bucket.
Next, make that bucket and the object in the bucket public. 
Launch an EC2 instance with SSH access
Copy the instance’s public ip address and SSH into your EC2 instance 
Run the following commands in your terminal 
sudo su 
yum update -y
yum install httpd -y
chkconfig httpd on
cd /var/www/html
wget (S3 object URL)
unzip (folder full name including extension)
mv (sub folder full name )/* .
service httpd start

Lastly copy your instance public ip and paste it in the web browser.

