# deployment

## <a name='deploying-concourse'></a>Deploying Single VM Concourse 

```
bosh -e my-env -d concourse deploy single-vm-concourse.yml \
  --vars-store ./concourse-deployment-vars.yml \
  -v concourse_static_vip=1.2.3.4 \
  -v concourse_external_url=https://concourse.example.com \
  -l certs.yml \
  [ -o operations/CUSTOMIZATION1 ] \
  [ -o operations/CUSTOMIZATION2 (etc.) ]
```
