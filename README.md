# Accessing Helm Chart from GitHub

First, clone the GitHub repository onto your machine using the following command:

    git clone https://github.com/Isha-Yasin/helm_chart.git
Download the Helm Chart (.tgz)
After cloning, navigate to the Releases section of the repository and download the .tgz file (Helm chart package) listed under "Assets."

# Install the Helm Chart
Run this command to install the Helm chart on your machine:

     helm install <release-name> /path/to/chart.tgz
Replace <release-name> with any name you want to give your release.
Replace "/path/to/chart.tgz" with the actual file path of the downloaded .tgz chart on your machine.
