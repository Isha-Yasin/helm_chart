# Installation :
You have must installed helm using this link

     https://helm.sh/docs/helm/helm_install/
or , if you have already helm you can skip
# Accessing Helm Chart with release :

Download release under the Github repo , then navigate to the directory .

# Add the Helm Repository
open terminal and run this command to add your Helm chart repository:

    helm repo add my-gripo https://raw.githubusercontent.com/<user name>/<repository>/<branch>/
like

    helm repo add my-gripo https://raw.githubusercontent.com/Isha-Yasin/helm_chart/main/

# Update the Helm Repositories
After adding the repository, they need to update Helm to get the latest version of the charts:

    helm repo update

# Install the Chart
Once the repository is added and updated, they can install the chart using the following command:

    helm install <release-name> my-gripo/<chart-name>

After installing verify that 

    kubectl get pod
    kubectl get svc

