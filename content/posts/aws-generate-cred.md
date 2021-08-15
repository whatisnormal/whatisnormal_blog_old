---
title: Generating Access keys in AWS
tags: [aws, security]
comments: true
date: 2021-08-15T14:00:00+01:00
---
It happens to me that from time to time, by security credentials when accessing AWS become invalid. Did I wrote a typo? Did I just forgot to update the file? Well multiple situations can trigger this.

# What are the steps then?

1. Go to security credentials on your account page.
2. Click on your name in the top right corner and select *My security credentials*
3. Generate access keys and add those to the _.aws/credentials file_
3. Export env variables by running:
    
    >    export AWS_ACCESS_KEY_ID=the generated key id
        
    > export AWS_SECRET_ACCESS_KEY=generated access key
    

