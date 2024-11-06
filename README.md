# ServerLordWeek1

## Explanation
- I have created a Dockerfile that sets up a python 3.9 environment, installs dependencies from requirements.txt, exposes the main.py file on port 5050, and runs this main.py file in the /app directory.
- The nginx.config file configures nginx as a reverse proxy with load balancing, forwarding requests to the instances of the Flask app.
- The docker-compose.yml file defines two services (flask application and nginx reverse proxy) with port mapping and dependencies. It sets up a shared network (app-network) between the two services.
- By default round robin algorithm is used for laod balancing the multiple instances of the Flask app, for fair distribution. 

## Demonstration
![Screenshot 2024-11-03 171516](https://github.com/user-attachments/assets/7e2ffb99-2c64-422e-b978-99bdcced2114)
![Screenshot 2024-11-03 171151](https://github.com/user-attachments/assets/9b62c7b9-9ff9-4566-b65e-07a2489d20bd)
![Screenshot 2024-11-03 172455](https://github.com/user-attachments/assets/b175286f-00de-4bc8-84e7-32c311e74d8c)
![Screenshot 2024-11-03 172524](https://github.com/user-attachments/assets/937678b7-ec0b-4324-a22c-096363e0d461)
![Screenshot 2024-11-03 172600](https://github.com/user-attachments/assets/cdd8c19f-9f54-4c27-93a2-cfcf4d5d6b7a)


## Best algorithm for cron job manager application
I believe that for a multi tenant SaaS like the cron job manager, the weighted round robin algorithm would best suit it's needs. This is because the higher priority jobs will be served more frequently. So this ensures the fair utilization of resources while keeping in mind the priorities. 
