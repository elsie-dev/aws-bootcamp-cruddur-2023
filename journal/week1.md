# Week 1 — App Containerization

## HOMEWORK/TECHNICAL TASKS

### Docker Containers
I created Dockerfiles for the frontend and backend then containerized both of them 
I then created a Dockercompose file as per the youtube Videos, did docker-compose up and build both containers.

Proof of work ![Backend Dockerfile](assets/Week%201%20docker%20backend%20container.JPG)

Proof of work ![Frontend Dockerfile](assets/Week%201%20frontend.JPG)

### Open API notification

I also set up notification for the crudder application

### Database containers

Set up both DynamoDB and Postgress Containers.Here's a screenshot to prove the same.

![Database Containers](assets/Week%201%20dynamo%20db.JPG)

## HOMEWORK CHALLENGES:

For this challenge here are some of the tasks l accomplished:
- [x] I learnt how to install Docker on my local machine and got the same outcome as codespace using.
- [x] On my local pc l run Dockerfile CMD as external script then pushed and tagged image to DockerHub
  - ![Proof of task](assets/Week1%20docker%20tag%20and%20push.JPG)
  
- [x] Creating an EC2 instance and installing Docker.
  - ![Proof of task](assets/Week1%20EC2%20docker%20installation.JPG)
  
- [x] Pulling my earlier pushed docker images in my DockerHub
  - ![Proof of task](assets/Week1%20pulled%20docker%20images.JPG)
  
- [x] I run Dockerfile as CMD script locally on my pc and redid the steps
  - ![Proof of task](assets/Week1%20docker%20tag%20and%20push.JPG)
  
# Issues encountered and how to solve:
- My Gitpod work space could not dispaly my files for the entire week had to shift to Codespaces after trying to create a new repo.
- While trying to push my images to DockerHub received request denied. I ued this documentation for guidance (stackoverflow)[https://stackoverflow.com/questions/41984399/denied-requested-access-to-the-resource-is-denied-docker]
 
