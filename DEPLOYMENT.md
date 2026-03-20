# Deployment Guide

## Deploying to Heroku

1. **Create a Heroku account** if you don't have one:
   - Go to [Heroku](https://signup.heroku.com/) to sign up.

2. **Install the Heroku CLI**: 
   - Follow the instructions [here](https://devcenter.heroku.com/articles/heroku-cli#download-and-install) to install the Heroku CLI.

3. **Log in to Heroku**:
   ```bash
   heroku login
   ```

4. **Create a new Heroku app**:
   ```bash
   heroku create <your-app-name>
   ```

5. **Set environment variables**:
   ```bash
   heroku config:set VAR_NAME=value
   ```
   - Repeat for each environment variable needed.

6. **Deploy your application**:
   ```bash
   git push heroku main
   ```

7. **Open your Heroku app**:
   ```bash
   heroku open
   ```

## Deploying to AWS

1. **Create an AWS account**:
   - Go to [AWS](https://aws.amazon.com/) to sign up.

2. **Install AWS CLI**:
   - Follow the [installation guide](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) to install AWS CLI.

3. **Configure your AWS CLI**:
   ```bash
   aws configure
   ```
   - Enter your AWS Access Key, Secret Key, region, and output format.

4. **Set environment variables** in AWS EC2 using IAM roles or user data scripts.

5. **Deploy your application** using Elastic Beanstalk, EC2, or ECS, based on your architecture preference.

## Deploying to DigitalOcean

1. **Create a DigitalOcean account**:
   - Go to [DigitalOcean](https://www.digitalocean.com/) to sign up.

2. **Create a Droplet**:
   - Choose the preferred image and size for your server.

3. **Connect to your Droplet via SSH**:
   ```bash
   ssh root@your_droplet_ip
   ```

4. **Set environment variables**:
   You can set them in your shell configuration file (e.g., `.bashrc`, `.bash_profile`) or by exporting them directly in the terminal:
   ```bash
   export VAR_NAME=value
   ```

5. **Deploy your application**: Upload your application files and start your server.

## Conclusion

Following these steps, you can successfully deploy your application to Heroku, AWS, or DigitalOcean. Make sure to adjust configurations as necessary based on your app requirements.

---

_Last updated: 2026-03-20 10:11:58 (UTC)_