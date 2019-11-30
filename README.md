# Image filtering microservice

## Table of Contents

* [Project Goals](#Project-goals)
* [Getting Started](#Getting-started)
* [Built with](#Built-with)
* [Authors](#Authors)
* [Acknowledgments](#Acknowledgments)

## Project goals

The goal of the project was to build a simple image filtering API deployed to a cloud provider. Key functionalities built:
- ```API applies a simple B&W filter to an image url sent via URL query```

The app was built from a boilerplate Express.js script provided in the course.

## Getting Started

You can clone the project files by running

```bash
git clone https://github.com/tamasdinh/cloud-image-filter.git
```

in your command line. This will download the entire repository to your computer, into a subfolder named ```cloud-image-filter``` in the folder from which you initiated cloning. Alternatively, you can download the repo as a ```zip``` file from the repo page.

Once you have the repo on your local machine, first you have to install dependencies by ```cd```-ing into the project folder and running:
```bash
npm install
```

You should obtain the url of an image on the web, e.g.:
* [Adorable kitten photo](https://timedotcom.files.wordpress.com/2019/03/kitten-report.jpg)

Once you have dependencies installed and a photo link obtained:

1. Try the API locally:
    - in the project folder, run ```npm run dev``` - this will start the development server locally at ```http://localhost:8082```
    - use Postman or any other method to send an HTTP GET request to the local server, e.g. you can paste ```localhost:8082/filteredimage?image_url=https://timedotcom.files.wordpress.com/2019/03/kitten-report.jpg``` into the address bar of your favorite browser
    - you will get back the filtered image of the adorable kitten photo mentioned as example above

2. Try the deployed service on AWS:
    - use Postman or any other method to send an HTTP GET request to ```AWS-Image-filter-dev.us-east-1.elasticbeanstalk.com```, e.g. you can paste ```AWS-Image-filter-dev.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://timedotcom.files.wordpress.com/2019/03/kitten-report.jpg``` into the address bar of your favorite browser
    - you will get back the filtered image of the adorable kitten photo mentioned as example above

```ENJOY!```

## Built With

* ```Javascript``` - :)
* [Node.js and Node Package Manager](https://nodejs.org/en/) - for handling dependencies and project configuration
* [Express.js](https://expressjs.com) - API server framework used
* [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/) - "Easy" app deployment for several frameworks, including Node.js.

## Authors

* **Tamas Dinh** - [LinkedIn profile](https://www.linkedin.com/in/tamasdinh/)