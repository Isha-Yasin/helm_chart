# Accessing Helm Chart from GitHub with 2 methods
# First method

First, clone the GitHub repository onto your machine using the following command:

    git clone https://github.com/Isha-Yasin/helm_chart.git
After cloning, navigate to the chart's directory and install it:

    helm install <release-name> ./helm_chart/test-helm
# Second method
# Download the Release
Open a web browser and go to your GitHub repository link (e.g., https://github.com/Isha-Yasin/helm_chart).
Click on the “Releases” tab, usually found on the right side of the page.
Look for the specific release you want (e.g., v1.0.0).
Click on the link to download the Helm chart .tgz file. This file is usually labeled with the version number.
Open a Terminal:
Download the Helm Chart (.tgz)
After cloning, navigate to the Releases section of the repository and download the .tgz file (Helm chart package) listed under "Assets."

# Install the Helm Chart
Run this command to install the Helm chart on your machine:

     helm install <release-name> /path/to/chart.tgz
Replace <release-name> with any name you want to give your release.
Replace "/path/to/chart.tgz" with the actual file path of the downloaded .tgz chart on your machine.
