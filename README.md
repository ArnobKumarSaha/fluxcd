## fluxcd


### Install Flux cli
`curl -s https://fluxcd.io/install.sh | sudo bash`

### Bootstrap Github repositories
Get a [Personal access token](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token).
`export GITHUB_TOKEN=<your-token>`

Run

```yaml
flux bootstrap github \
--owner=Arnobkumarsaha \
--repository=fluxcd \
--path=cluster \
--branch=master \
--personal
```