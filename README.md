


# build multiple small gce instances with no external ip for demo #



openssl pkcs12 -in skc-gce-ansible-01-803c07f76f2b.p12 -passin pass:notasecret -nodes -nocerts | openssl rsa -out pkey.pem



used to check your yml before you run it
`--syntax-check --list-tasks`

`ansible-playbook --syntax-check --list-tasks build.yml`


`ansible-playbook  build.yml`



ping the systems

`ansible all -m ping`

`ansible test -m setup`

`ansible test -m command -a "uptime"`

`ansible test -m script -a ./files/foo.sh`


**** ssh into system
gcloud compute ssh skc-1 --zone us-central1-a



