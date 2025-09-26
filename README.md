# DevOps Mini Test

Welcome 👋 This repo is a simple Python Flask app with one API endpoint.
- You will be given an access to an aws account for the VPN questions
- You are free to start with any number.
- You are free to ask any questions for clarity
- Kindly delete all resources created for task 1 after the test.
- The task 1 should be done in eu-west-1 region

Your tasks:

### 1. VPN
- Create a VPN Tunnel in AWS and connect to the following configuration
####  Conn
        PeerIP=146.190.120.240
        Host=10.48.0.6/32
####   phase 1 (IKE)
       keyexchange=ikev2
       ike=aes256-sha1-modp2048
       ikelifetime=3600s
####   phase 2 (ESP)
       esp=aes256-sha1
       keylife=3600s


### 2. Docker
- Write a `Dockerfile` that runs this app on port 5000.

### 3. Docker Compose
- Create a `docker-compose.yml` with:
  - This app service
  - A Postgres service (use `postgres:15-alpine`)
- Connect the app to Postgres (set DB env vars).

### 4. CI/CD
- Write a GitHub Actions workflow:
  - Run tests (`pytest`)
  - Build Docker image
  - Deploy via docker-compose



Good luck 🚀
# devops-test
