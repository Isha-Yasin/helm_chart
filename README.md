# Accessing Helm Chart from GitHub with 2 methods
# First method

First, clone the GitHub repository onto your machine using the following command:

    git clone https://github.com/Isha-Yasin/helm_chart.git
After cloning, navigate to the chart's directory and install it:

    helm install <release-name> ./helm_chart/test-helm
# Second method
# Download the Release
Open a web browser and go to your GitHub repository link (e.g., https://github.com/Isha-Yasin/helm_chart).<br> 
Click on the “Releases” tab, usually found on the right side of the page.<br>
Click on the link to download the Helm chart .tgz file (Helm chart package) listed under "Assets." This file is usually labeled with the version number.<br>
By  terminal check what's inside .tgz file run this command:

    tar -xvzf <<path/of/.tgz>>

Add the Helm Repository
open terminal and run this command to add your Helm chart repository:

    helm repo add my-gripo https://raw.githubusercontent.com/<user name>/<repository>/<branch>/
like

    helm repo add my-gripo https://raw.githubusercontent.com/Isha-Yasin/helm_chart/main/

Update the Helm Repositories
After adding the repository, they need to update Helm to get the latest version of the charts:

    helm repo update

Install the Chart
Once the repository is added and updated, they can install the chart using the following command:

    helm install <release-name> my-gripo/<chart-name>

After installing verify that 

    kubectl get pod
    kubectl get svc
accessing application run this command

    minikube svc nginx
