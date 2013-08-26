Photo Blog = Phlog

-------------------------------------------

Development Environment Setup Instructions:

1) bundle install

2) rake db:setup

3) Create an AWS S3 bucket (http://docs.aws.amazon.com/AmazonS3/latest/gsg/CreatingABucket.html)

4) Update your config/application.yml file with these three items related to your S3 bucket (With your own access key, secret access key, and bucket name, duh..)

AWS_ACCESS_KEY_ID: "89237987589437"

AWS_SECRET_ACCESS_KEY: "euhy892759847589"

AWS_S3_BUCKET: "your-bucket-name"

5) rails s

6) Start up the redis database by typing below command in another terminal prompt (leave it running):

redis-server /usr/local/etc/redis.conf

7) Start up the background process by typing below command in another terminal prompt (leave it running):

bundle exec sidekiq

-------------------------------------------

Heroku Deployment link:

http://phlog.herokuapp.com/
