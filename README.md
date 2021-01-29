# IBM AI Enterprise Workflow Capstone
Files for the IBM AI Enterprise Workflow Capstone project. 

## Part 1

### Case study part 1

See notebook part 1 for Data ingestion, EDA and visualizations.

## Part 2

### Case study part 2

See notebook part 2 for modeling selection, 3 algorithms were compared. RandomForestRegressor, GradientBoostingRegressor and LassoCV

## Part 3

To start the flask application locally, run the following command:

python app.py

### tests

To run api tests:

python unittests/ApiTests.py

To run ModelTests:

python unittests/ModelTests.py

To run LoggerTests:

python unittests/ModelTests.py

To run all test:

python runAllTests.py

### Training the model

The modelscript used is model.py from part 2.
See saved country specific models under /models


### Build the Docker image and run it
Step one: build the image (from the directory that was created with this notebook)

    ~$ cd docker-tutorial
    ~$ docker build -t example-ml-app .
Check that the image is there.

    ~$ docker image ls
You may notice images that you no longer use. You may delete them with

    ~$ docker image rm IMAGE_ID_OR_NAME
Run the container

docker run -p 8080:8080 example-ml-app

### Monitoring performance

See notebook MonitorPerformance

## Questions answered
Are there unit tests for the API?
Are there unit tests for the model?
Are there unit tests for the logging?
Can all of the unit tests be run with a single script and do all of the unit 1. tests pass?
Is there a mechanism to monitor performance?
Was there an attempt to isolate the read/write unit tests from production 1. models and logs?
Does the API work as expected? For example, can you get predictions for a 1. specific country as well as for all countries combined?
Does the data ingestion exists as a function or script to facilitate 1. automation?
Were multiple models compared?
Did the EDA investigation use visualizations?
Is everything containerized within a working Docker image?
Did they use a visualization to compare their model to the baseline model?

