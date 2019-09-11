# Demo of IBM's Watson Studio AutoAI to Predict Titanic's survivors

## A 3-minute video of the demo can be downloaded from [here](https://ibm.box.com/s/62ngb7y0cppespkty308a3u9r2jdjg3o). The video uses the newest version of the AutoAI UI that is not in production yet. Therefore, there will be minor chnages in the UI between the video and the demo that you can build yourself. 

### Here are the step-by-step instructions to build the demo on your own:

1. If you don't an IBM cloud account, navigate to <https://cloud.ibm.com/registration> to create one. Otherwise, sign-in using your IBM coud account here: <https://cloud.ibm.com/login>

1. Search for `Watson Studio` on the search bar of IBM's cloud 
 ![](https://github.com/IBMDataScience/autoai/blob/master/images/search%20WS.png)
  
1. Create a `Watson Studio` instance (it's a service on IBM cloud) by clicking the `Create` button on the bottom right  ![](https://github.com/IBMDataScience/autoai/blob/master/images/create%20WS%20instance.png)

1. Click `Get Started` ![](https://github.com/IBMDataScience/autoai/blob/master/images/get-started.png)
 
1. The first step to start using WS is to create a project, click  `Create a project` ![](https://github.com/IBMDataScience/autoai/blob/master/images/create-project.png)
 
1. Now we want to create a project from scratch, so click `Create an empty project` ![](https://github.com/IBMDataScience/autoai/blob/master/images/create-empty-project.png)

1. If you already have storage, name your project and click `Create` (go to the next step). Otherwise, add storage by clicking `Add` then `Create`,  `Confirm`. Then `Refresh` the project creation page to get your storage service attached to your project. Now click `Create` to create your project. ![](https://github.com/IBMDataScience/autoai/blob/master/images/add-storage.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/create-storage.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/confirm-storage.png) ```
A project is the key structure of Watson Studio to develop data science experiments. It is easy to add collaborators and share dataset, data connections and a big family of analytical assets (modeler flows, jupyter notebooks, data refinery flows, Watson services, among others). Feel free to spend some time exploring the different parts of a project. ```

1. Let's add data to the project! Download to your laptop the public Titanic dataset from the Stanford's webpage: https://web.stanford.edu/class/archive/cs/cs109/cs109.1166/stuff/titanic.csv

1. From your Watson Studio project, click the data icon on the top right to drop the `titanic.csv` or browse. ![](https://github.com/IBMDataScience/autoai/blob/master/images/data-icon.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/drop-or-browse.png)

1. Now click on `Assets` to verify that your data was loaded correctly. 
![](https://github.com/IBMDataScience/autoai/blob/master/images/assets.png)

1. Ready for some AI? Click on `Add to project` blue icon on the top and click `AutoAI Experiment` ![](https://github.com/IBMDataScience/autoai/blob/master/images/add-to-project.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/autoai-icon.png)

1. If you already have a Watson Machine Learning (WML) service, just name your experiment and click `Create` (go to the next step). Otherwise, add a WML service by clicking `Associate a Machine Learning instance` then `Create` and `Confirm`. Now you can `Reload` the experiment creation page to get your WML service attached. Click `Create`. ![](https://github.com/IBMDataScience/autoai/blob/master/images/add-wml.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/create-experiment.png)

1. AutoAI only needs to be pointed to a dataset and a column to predict in the dataset. Easy. LEt's choose the `titanic.csv` after clicking the `Select from project` blue button. Click `Select asset`. ![](https://github.com/IBMDataScience/autoai/blob/master/images/select-data-from-project.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/select-titanic.png)

1. Let's select the column to predict the titanic survivors: `Survived` which is a binary (takes only the values 0 = not survived or 1 = survived). The quality metric is automatically selected for you: the ROC AUC is the standard quality metric for binary classification problems. Click `Run experient`. ![](https://github.com/IBMDataScience/autoai/blob/master/images/survived-run-experiment.png)

1. The rest is waiting for AutoAI to train several pipelines and show you the best in the leaderboard. You should see the first trained pipeline in less than one minute. Once the run is completed, we can check the pipeline leaderboard to see the winner. More over, we can click the pipeline to drill down into quality metrics, confusion matrix, model information and feature importance. In this example, the most important feature to explain Titanic survivors was the sex of the passenger. ![](https://github.com/IBMDataScience/autoai/blob/master/images/pipeline-leaderboard.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/model-evaluation.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/conf-matrix.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/model-information.png) ![](https://github.com/IBMDataScience/autoai/blob/master/images/feature-importance.png) 

1. To save your pipeline (and deploy as a REST API) click `Save as model` on the top right and `Save`. This action will save your model as an asset in your project. ![](https://github.com/IBMDataScience/autoai/blob/master/images/save-as-model.png)
