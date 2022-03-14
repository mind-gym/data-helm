# data-helm
This is a general helm chart for dashboards
## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

  helm repo add dashboard https://mind-gym.github.io/data-helm/

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
`dashboard` to see the charts.

To install the dashboard chart:

   helm upgrade -i --timeout 0 -f values.yaml `product`-`actual-name-of-dashboard` dashboard/dashboard

To uninstall the chart:

    helm delete `product`-`actual-name-of-dashboard`