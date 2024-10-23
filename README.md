# ServerLordWeek1


1. Fork this repository
2. Dockerise the python app and expose it on port 5050 using port mapping 
3. Make >2 instances of the application and create a docker network using docker-compose containing all the instances and a nginx proxy that distributes the load and is visible on port 80 of host machine
4. Start with a round robin algorithm for load balancing and explore other options
5. What algorithm do you think will best suit the needs of a multi tenant SAAS like our cron job manager application? Give your justification in the README.
6. Give a demonstration of the whole set-up (steps 3-5) through screen shots and brief explanations.

Resources :
[Docker](https://www.youtube.com/watch?v=Ud7Npgi6x8E)

[Docker compose](https://www.youtube.com/watch?v=HGKfE-cn9y4&t=111s)

[Installation](https://medium.com/@tomer.klein/step-by-step-tutorial-installing-docker-and-docker-compose-on-ubuntu-a98a1b7aaed0https://www.youtube.com/watch?v=HGKfE-cn9y4&t=111s)

[Inspiration for our application](https://healthchecks.io/)
   
