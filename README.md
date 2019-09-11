# Demo of IBM Watson Studio AutoAI's Tool 

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

1. 
