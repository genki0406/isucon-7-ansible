## init

```
pip install pipenv
pipenv install
```

## deploy

```
# app
pipenv run ansible-playbook -i inventory app.yml -c ssh -u ubuntu --private-key=~/.ssh/isucon-play-ground.pem

# web
pipenv run ansible-playbook -i inventory web.yml -c ssh -u ubuntu --private-key=~/.ssh/isucon-play-ground.pem

# db
pipenv run ansible-playbook -i inventory db.yml -c ssh -u ubuntu --private-key=~/.ssh/isucon-play-ground.pem
```